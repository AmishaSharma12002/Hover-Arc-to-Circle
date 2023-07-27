# Hover-Arc-to-Circle

## NOTE: Make sure to download any image that you want for this effect or add a web link in the img tag (HTML CODE).
HTML Code:

1. `<!DOCTYPE html>`: The doctype declaration specifies that this is an HTML5 document.
2. `<html>`: The opening tag for the HTML document.
3. `<head>`: The head element contains meta-information about the document, such as the title and links to external resources.
4. `<meta name="viewport" content="width=device-width, initial-scale=1.0">`: Sets the viewport properties for responsive design, ensuring proper rendering on various devices.
5. `<title>hover</title>`: Sets the title of the web page to "hover".
6. `<link rel="stylesheet" href="styles.css">`: Links the external CSS file named "styles.css" to the HTML document.
7. `</head>`: Closes the head section of the document.
8. `<body>`: The body element contains the visible content of the document.
9. `<img src="couple.png" height="300px">`: Inserts an image with the source "couple.png" and sets its height to 300 pixels.
10. `</body>`: Closes the body section of the document.
11. `</html>`: Closes the HTML document.

CSS Code:

1. `img {`: Targets all `<img>` elements in the HTML.
2. `--m: ...`: Defines a custom CSS variable (--m) that contains multiple radial-gradient values separated by commas. These gradients create a blend from solid black to transparency on both sides of the image. The variable is defined but not applied directly to any element.
3. `-webkit-mask: var(--m);`: Applies the custom CSS variable (--m) as the mask to the image for browsers that use the WebKit rendering engine (e.g., Safari).
4. `mask: var(--m);`: Applies the custom CSS variable (--m) as the mask to the image for other browsers that support the CSS mask property.
5. `filter: grayscale(.5);`: Applies a grayscale filter to the image, reducing its color saturation by 50%.
6. `transition: .3s linear;`: Specifies the transition property for the image, making the transition smooth with a duration of 0.3 seconds and a linear timing function.
7. `cursor: pointer;`: Changes the cursor to a pointer when hovering over the image, indicating it is interactive.
8. `}`: Closes the CSS rule for the `<img>` element.

9. `img:hover {`: Targets the `<img>` element when it is being hovered over by the cursor.
10. `-webkit-mask-position: 7.5% 50%, 92.5% 50%;`: Changes the position of the mask on hover to create the transition from the arc shape to a circle shape. The two values correspond to the x-axis and y-axis positions of the gradients, respectively.
11. `mask-position: 7.5% 50%, 92.5% 50%;`: Same as above but for non-WebKit browsers.
12. `filter: grayscale(0);`: Removes the grayscale filter on hover, restoring the image's original colors.
13. `}`: Closes the CSS rule for the `<img>` element when it is being hovered over.

