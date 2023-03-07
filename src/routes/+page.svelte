<script>

let seed = '';

// Generates a 7 random letter seed from a-z and A-Z
const generateSeed = () => {
    const allLetters = 'abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ';
    for(let i = 0; i < 7; i++) {
        seed += allLetters.charAt(Math.floor(Math.random() * allLetters.length));
    }
    generateRandomValues(seed);
    return seed;
}

// https://stackoverflow.com/questions/901115/how-can-i-get-query-string-values-in-javascript
// https://www.youtube.com/watch?v=7BbL2PZ5394
// Generates URL
const addSeed = () => {
    const url = 'http://127.0.0.1:5173/?';
    const obj = { s: seed };
    const searchParams = new URLSearchParams(obj);
    window.location.href = url + searchParams;
    readSeed();
}
// Read just the seed part of the URL
const readSeed = () => {
    const getURL = new URLSearchParams(window.location.search);
    return getURL.get('s');
}

// Generate Random Values for Seed
const generateRandomValues = (seed) => {
    let seedVal = 0;
    const values = [];
    for (let i = 0; i < seed.length; i++) {
        seedVal += seed.charCodeAt(i);
        values.push(seedVal)
    }
    console.log(values);
    
}

</script>

<button on:click={() => { generateSeed(); addSeed(); }}>7 random letters</button>
<!-- <p>{letterStr}</p> -->


<style>

</style>