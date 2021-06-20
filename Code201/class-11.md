# Class 11

## **HTML IMAGES**

> Images can improve the design and the appearance of a web page. <small> W3 Schools.</small>

* we specify the dimensions of images using CSS and it will be very helpful if we used the same image sizes.

* Images can be aligned both horizontally and vertically using CSS.

* we can use a background image behind the box created by any element on a page.

* Background images can appear just once or be repeated across the background of the box.

* we can create image rollover effects by moving the background position of an image.

* To reduce the number of images the browser has to load, you we create image sprites.

```html

<img src='Source Location' alt="alternative text , can be read by the page narriators" id="imgID">

```
## Background Image

its a property in CSS applies a graphic (e.g. PNG, SVG, JPG, GIF, WEBP) or gradient to the background of an element. There are two different types of images we can include with CSS: regular images and gradients.

By default, a background-image is placed at the top-left corner of an element, and repeated both vertically and horizontally. 

which is the total size of the element, including padding and border . 



## Image Sprites

* image sprite is collection of images put into a single image.

* A web page with many images can take a long time to load and generates multiple server requests.

* Using image sprites will reduce the number of server requests and save bandwidth.

- Example 
```html
<img id="sprites" src="transparent.gif"> 

```

- Only defines a small transparent image because the src attribute cannot be empty. 

The displayed image will be the background image we specify in CSS

```css
width: 46px; height: 44px;
background: url(img_navsprites.gif) 0 0;
left 0px, top 0px
```
 - Defines the portion of the image we want to use
 - Defines the background image and its position 


## Image RollOver

images involve changing one thing to another thing when the cursor hovers over it. 

If you use an image for a link, for example, you could swap that image with another one when the cursor hovered .

How its done :

* he onmouseover attribute is used to change the source file URL of the image when the user moves mouse pointer on the image. The onmouseout attribute is used to change the source file URL of the image when the user moves mouse pointer out of the image.

```html

<img src="inmg..." onmouseover="this.src='img2...'" onmouseout="this.src='img3...'" />

```


[**Back**](https://odehabuzaid.github.io/reading-notes/)                     | [**TOP**](##HTML-IMAGES) |

