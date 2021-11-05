# Images in p5

Today we will be learning how to render images in p5! Up to this point, we have been stuck with the shapes and built in components that p5 has provided (ellipse, rect, triangle, etc.). Today we will be looking at how we can begin to render other media from the internet into our programs.

## `function preload()`
All of the media (images, sounds, gifs, etc.) that we upload to repl.it is stored on a server, not on our computer. This means it takes time to go get these images. JavaScript doesn't wait for these things to load, but instead continues working through the lines of code that we have written.

The `preload` function is a special function in p5 that allows us to tell JavaScript to STOP and wait for the certain elements to load before proceeding with the remainder of the code.

```javascript
var img;
function preload(){
	// Loads the file with the name birch.png
	img = loadImage("birch.png")
}
```

Once prelod has been executed we can render our image using the variable that we stored the image in and the `image` function. The image function asks for the image, x coordinate, and y coordiate. The width and height can be provided as well if you wish to adjust them.

```javascript
function draw(){
	// Load the image called img at 50, 50 with a width of 100px and a height of 200p
	image(img, 50, 50, 100, 200)
}
```

## Saving and Loading Images Into Repl.it

**To save an image from Google Images, you should**:

1. Look for transparent images on Google
2. Two finger click on the image when found and click “Save Image As”
3. Give the image a SIMPLE name

![](/assets/GoogleImage.gif)

To upload an image to repl.it you should follow the gif below:

![](/assets/replit.gif)

## TASK

**GOAL**: GOAL: You’re going to design your own digital scene using images that you have found on Google Images.

**Examples**: 
- “A day in the forest”
- “A street in New York”
- “Under the sea”
- “Basketball in the park”

Need ideas? [Use one of these prompts!](https://artprompts.org/situation-prompts/)
