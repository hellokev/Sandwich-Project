# Sandwich Generator

Generate random sandwiches

# Development Guide

1. Install NodeJS

2. Fork the repository

3. Install dependencies
```bash
npm install
```

4. Run the project locally
```bash
npm run dev
```

5. Make some changes

6. You can save your github credentials by running
``` bash
git config --global credentials.helper store
```
7. Generate a github access token ([guide](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token))

8. Add your changes using 
```bash
git add <files>
```

9. Commit your changes using 
```bash
git commit -m "commit message here"
```

10. Push your changes to your fork
```bash
git push
```

11. When asked for your credentials, use your GitHub username and the password will be the access token you generated from step 7 

12. Create pull request (should show up when you visit your fork on github.com)

# How to help with pixel art assets

## Setting up Aseprite

1. Install Aseprite. You can buy this for $20 or apparently you can just compile the repo and get it for free that way? Not sure how that works, but if you can figure it out do it! (if you ever wanna try making with pixel graphics this is the go-to app)

2. Create a new file and name it in the same way I have for the examples. Set the dimensions to 32 x 32 (good amount of resolution but still a very pixel art feel)

3. Check the dimension_ref.png for guidelines on the placement of your sprite. Maybe make it a tab in your Aseprite for easy access. Draw within where the green square is, 20-ish pixels from the bottom


## Quick intro to Aseprite

* `b` for Brush Tool
* `e` for Erase Tool
* `g` for Bucket Tool

* that's all you'll realistically need, but check out the Aseprite Quick Reference for more...

## Making a sprite

0. Choose a condiment, ingredient, or bread type

1. Make a blob in the rough shape of the item you want in a base color (within specified dimensions of 20x32)

2. To change shades of a color,

* For DARKER colors: Move HORIZONTAL slider slightly TOWARDS BLUE, move the SQUARE color picker above it slightly down towards black
* For LIGHTER colors: Move HORIZONTAL slider slightly TOWARDS YELLOW, move the SQUARE color picker above it slightly up towards white
(if that doesnt make sense don't worry too much about it)

* You should aim for around 3-4 shades of color in your sprite; we want readability, we don't care about detail as much

3. Add details, subtract details, mess around with it! 

* as much as possible, try to stylistically follow the examples I have in `assets/final_pngs`

* use reference! look up: the name of the ingredient you're using + pixel art

* if you make a bun, try to make the top and bottom bun of the same type of bread for continuity's sake. Title them as `<breadname>_top.asperite` and `<breadname>_bottom.aseprite`. Also we're gonna keep bun separate from ingredients(the middle parts of sandwich)

4. When you are satisfied with your work, do save your file as a `.aseprite` file and put it in the `aseprite_files` folder. From there, git add, git commit, git push, then pull request.

5. rinse and repeat! we're gonna want a lot of these eventually, so quantity over quality! I will also tidy up, fix color, and export as png all the `.aseprite` files so don't worry if it's not perfect!

NOTE: When this gets put into the final project, it will likely be blurry because it's so small. I think these docs should help:
https://developer.mozilla.org/en-US/docs/Games/Techniques/Crisp_pixel_art_look

