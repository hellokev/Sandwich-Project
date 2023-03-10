<svelte:head>
	<title>Sandwhich Generator</title>
	<meta name="description" content="Svelte demo app" />
</svelte:head>

<section>
	<h1>
		Sandwhich Generator
	</h1>

	<h2>
		Welcome to our website, which generates random sandwiches! 
		We are passionate about sandwiches and believe they are more than just a meal. 
		They are a work of art that brings people together.
		Our website offers a unique and fun experience for sandwich lovers. 
		With just a click of a button, you can generate a random sandwich recipe that includes a variety of ingredients,
		from classic deli meats and cheeses to exotic sauces and vegetables. You will never run out of new sandwich ideas.
	</h2>

	<button>Generate a new sandwich!</button>

</section>

<style>
	section {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		flex: 0.6;
	}

	h1 {
		width: 100%;
	}

	.welcome {
		display: block;
		position: relative;
		width: 100%;
		height: 0;
		padding: 0 0 calc(100% * 495 / 2048) 0;
	}

	.welcome img {
		position: absolute;
		width: 100%;
		height: 100%;
		top: 0;
		display: block;
	}
</style>
