## Class 01

## **`Foundations of Software Development`**

---
**before building a web site , some terms must be defined and clarified**

- BROWSER : a software that allow us to access a web page.

- WEB SERVER : when asking browser for a web page , the request sent to `web server` that where the website files and data stored.( Hosted )

- DEVICES : desktop computers,
laptops, tablets, and mobile
phones. , not to forget that every one of them have different specifications, which will not make them display the content of a web browser the same. 


>  All websites uses HTML,CSS , But CMS offen add a few more technology to the mix.




|  |   | 
| ---            | :--        |   
|     What we See    |browser  sends a request to a server that I want this content.  > The server knows everything of what response it should send for every request. Hence, the server responds back. << This response contains every information that browser requested like web `page`, status-code, cache-control, etc. >>  the browser renders the content that has been requested and present them on screen|  
|     How `page`  created | in small web site it will be just the an html,css , but in large CMS more complex technology involved in producing that HTML , CSS and sent to the browser for rendering 


## **Structure OF a web Page**

> and it means how the page is set up, 

HTML : Hypertext markup language , while 

Hypertext : allow us create links that visitors can move from one page to another and from section to another ... 

The Markup language allow us to annotate text, and these annotations provide additional meaning to the contents of a document.


**HTML Describes
the Structure
of Pages**

`HTML code is in blue, and the text you see on screen
is in black.`

```html
<html>
<head></head>
<body>
 <h1>This is Heading 1</h1>
 <p> this is a sample paragraph.<p>
 <h2>This is a Sub-Heading</h2>
 <p>Here you can see a sub-heading.</p>
</body>
</html>
```


> ` keep in mind we structure web pages to make them easer to understand and give them better looking`

HTML Uses Elements `<html>` to Describe the Structure of Pages
Each element has an opening tag and a closing `</html>` tag.

tags act like containers.

Tells you information that lies between their opening and closing tags

The opening tag  `<html>` indicates that anything between it and a closing `</html>` tag is HTML code.

The  `<body>` tag indicates that anything between it and the closing `</body>` tag should be shown inside the main browser window.

 `<  'the tag purpose'   >  ....... <   /' End of tag purpose'> `

**Attributes**
---
They  provide  information's about the contents of an `Elements`

`Attributes` appear on the opening tag of the `element`

containing two parts   a name and a Value  separated by equal = sign 

Name  = Value

eg.  `<p lang="en-us">Paragraph in English</p>`

Most attribute values are either pre-defined or follow a specific / fixed  format.

# **Extra Markup**
> DOCTYPES tell browsers which version of HTML you
are using.

HTML 5 
```html
<!DOCTYPE html>
```

HTML 4
```html
<!DOCTYPE html PUBLIC "-//W3C//DTD HTML 4.01 Transitional//EN" "http://www.w3.org/TR/html4/loose.dtd">
```

Transitional XHTML 1.0
```html
<!DOCTYPE html PUBLIC
"-//W3C//DTD XHTML 1.0 Transitional//EN"
"http://www.w3.org/TR/xhtml1/DTD/
 xhtml1-transitional.dtd">
```

Strict XHTML 1.0
```html
<!DOCTYPE html PUBLIC
"-//W3C//DTD XHTML 1.0 Strict//EN"
"http://www.w3.org/TR/xhtml1/DTD/
 xhtml1-strict.dtd">
```

XML Declaration
```html
<?xml version="1.0" ?>
```

> You can add comments to your code between the `<!-- and -->` markers.

- Single line comment
```html
<!-- start of introduction -->
<h1>Current Exhibitions</h1>
<h2>Olafur Eliasson</h2>
<!-- end of introduction -->
```

- Multi-line comment
```html
<!-- 
<h1>Current Exhibitions</h1>
<h2>Olafur Eliasson</h2>
end of introduction -->
```
> The id and class attributes allow you to identify particular elements.

```html
<p id="pullquote">Lorem Ipsum, Neque porro quisquam est qui dolorem ipsum quia dolor sit amet, consectetur, adipisci velit.
</p>
<p class="important">Lorem Ipsum, Neque porro quisquam est qui dolorem ipsum quia dolor sit amet, consectetur, adipisci velit.
</p>
<h1 class="important"> Heading </h1>
```
> The `<div>` and `<span>` elements allow you to group
block-level and inline elements together.

```html
<div id="header">
<img src="images/logo.png" />
<ul>
   <li><a href="index.html">Home</a></li>
</ul>
</div><span class="pics">new
 picture</span>

<!-- end of header -->
```
<em> Using an id or class attribute on the `<div>` element, 
means that you can create CSS style rules for that div like the background color or position , size …. 

It can also make it easier to follow your code if you have used elements to hold each section of the page.</em>

**Inline Elements** 

elements that will always appear to continue on the same line as their neighbouring elements. |
`<a>, <b>, <em>, and <img>` | 

 **iframes Elements** 

> `<iframes>` cut windows into your web pages through
which other pages can be displayed.
content of the iframe is an html page
- this code withh Embed a video from youtube into your page.  
```html
<iframe width="560" height="315" src="https://www.youtube.com/embed/7_LPdttKXPc" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
```
**Informations About
Your Pages** 

> the `<meta>` place is inside the `<head>` element and contains information about the web page.
- `<meta>` is not visible to the user.
- `<meta>`  tells search engines about your page, who created it,and whether or not it is time sensitive. (If the page is time sensitive, it can be set to expire.)
- `<meta>` does not have a closing tag.
It uses attributes to carry the information - most common { attributes are the name and content}

The value of these attributes can be any thing : most common used values : 

**Description**  : This contains a description of the page.


**Keywords** : This contains a list of commaseparated words that a user might search on to find the page. 


**Robots**  : indicates whether search engines should add this page to their search results or not. A value of noindex can be used if this page should not be added. A value of nofollow can be used if search engines should add this page in their results but not any pages that it links to.


```html
<head>
 <title>Information Technology</title>
 <meta name="description"
 content="An Essay on AI " />
 <meta http-equiv="author"
 content="Jon Duckett" />
 <meta http-equiv="pragma"
 content="no-cache" />
 <meta http-equiv="expires"
 content="Fri, 04 Apr 2014 23:59:59 GMT" />
</head>
```

... To be Continued 