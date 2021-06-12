## Class 02

## **`HTML Text, CSS Introduction, and Basic JavaScript Instructions`**

---

**Headings and paragraphs**

> tags provide extra meaning and allow browsers to show users the appropriate structure for the page.

Structural markup VS Semantic markup

the elements that you can use to
describe both headings and paragraphs

which provides extra information; such
as where emphasis is placed in a sentence, that something
you have written is a quotation (and who said it), the
meaning of acronyms, and so on

HTML headings
HTML defines six levels of headings. A heading element implies all the font changes, paragraph breaks before and after, and any white space necessary to render the heading. The heading elements are H1, H2, H3, H4, H5, and H6 with H1 being the highest (or most important) level and H6 the least.

Paragraphs
The HTML `<p>` element defines a paragraph.

A paragraph always starts on a new line, and browsers automatically add some white space (a margin) before and after a paragraph.

HTML bold
To make text bold in HTML, use the `<b>… </b>` tag or `<strong>… </strong>` tag. Both the tags have the same functioning, but `<strong>` tag adds semantic strong importance to the text.

html italic
To make text italic in HTML, use the `<i>… </i>` tag or `<em>… </em>` tag. Both the tags have the same functioning, but `<em>` tag is a phrase tag, which renders as emphasized text.

html emphasis
The HTML `<em>` element marks text that has stress emphasis. The `<em>` element can be nested, with each level of nesting indicating a greater degree of emphasis.

html superscript
The `<sup>` tag defines superscript text. Superscript text appears half a character above the normal line, and is sometimes rendered in a smaller font. Superscript text can be used for footnotes, like WWW[1].

html subscript
The `<sub>` tag defines subscript text. Subscript text appears half a character below the normal line, and is sometimes rendered in a smaller font. Subscript text can be used for chemical formulas, like H2O.

White Space
what is white space collapsing :

all white spaces in html document considered as a single space .

Line Breaks & Horizontal Rules
`<br>` makes line break and continue rendering what comes after it in a new line

`<hr>` draws a horizontal line on the page

A semantic element clearly describes its meaning to both the browser and the developer.

The HTML `<blockquote>` element defines a section that is quoted from another source.

```html
<blockquote cite="http://www.worldwildlife.org/who/index.html">
For 50 years, WWF has been protecting the future of nature.
The world's leading conservation organization,
WWF works <q> in 100 countries and is supported by
1.2 million members </q>in the United States and
close to 5 million globally.
</blockquote>
```

`<q>`
The `<q>` element is used for
shorter quotes that sit within
a paragraph.

`Abbreviations & Acronyms`

`<abbr>`
The `<abbr>` tag defines an abbreviation or an acronym, like "HTML", "CSS", "Mr.", "Dr.", "ASAP", "ATM".

Citations &
Definitions

The `<cite>` tag defines the title of a creative work (e.g. a book, a poem, a song, a movie, a painting, a sculpture, etc.). Note: A person's name is not the title of a work. The text in the `<cite>` element usually renders in italic.

Basic JavaScript Instructions
---

JavaScript Objects defined as a collections of key / value pairs.

The values consist of properties and methods,
may contain all other JavaScript data types, such as strings, numbers, and Booleans.

JavaScript objects descend frm parent Object constructor.
Object has has useful built-in methods .
Object methods are used directly on the Object constructor,
and use the object instance as a parameter.
This is known as a static method.

The Object class represents one of JavaScript's data types.

used to store various keyed collections .

Objects can be created using the Object() constructor or the object initializer

How to use the Objects and their methods

![Example](https://i.imgur.com/1TAQdYS.png)

> JAVASCRIPT RUNS WHERE IT IS FOUND IN THE HTML

#### why its best to keep javascript code in its own Js file ?

we use `<Script>` element when we want to load the java script file.

script : list of commands in a form of (statements) that are executed by a certain program or scripting engine.

comments : The js comment `<tag>` is used to add text to an HTML document without including that text in the Web page.

```js
// Single line Comment

/*
m
u
l  i   n  e Js Comment
t
i
*/
```
   [**Back**](https://odehabuzaid.github.io/reading-notes/)                     | [**TOP**](#Class-02) |