# Class 12

## **Local Storage**

Local storage is part of the HTML5 Web Storage API.

it allows storing data in the browser. but unlike cookies sessions it isn’t sent back to the server. All data stays on the client side, and can currently store from 2MB to 10MB. This limit is tied to the specific browser, protocol (HTTP or HTTPS), port, and top level domain in use.


>![Jsimg](https://lh3.googleusercontent.com/proxy/0w-evqIoeuqAe7x8oQHPu_ixEUz1v0lbc3B1ZKRH-obWdSvuJRQhP4201kyOFtuR1_T9QwkpguR2x2MV1_BQoerXyIF_TT1JuFsISZcHYPxjRbYa
)
<small> local storage</small>

### Potentially Dealbreaking Downsides:

* Cookies are included with every HTTP request, thereby sending data unencrypted over the internet unless your entire web application is served over SSL.
* Cookies are limited to about 4 KB of data — enough to slow down your application.


## BEFORE HTML5:

there was userData which allows pages to store up to 64 KB of data per domain, in an XML-based structure.
intranet sites:Trusted domains can store 10 times that amount.

Local Shared Objects allows Flash objects to store up to 100 KB of data per domain.


## HTML5 STORAGE

a way for web pages to store data in key/value pairs locally, within the client web browser.

STORAGEEVENT OBJECT

> ![Jsimg](./code201/res/localstorage.PNG)

examples and usage : 

Remove single desired key

```js
localStorage.removeItem(key); 

```
Insert A Single Row:
```js

localStorage.setItem("key", "value");

```
Get A Single Row:
```js

let getValue = localStorage.getItem("key");

```
Remove All Rows:

```js

localStorage.clear();

```
[**Back**](https://odehabuzaid.github.io/reading-notes/)                     | [**TOP**](##Local-Storage) |