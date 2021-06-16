# Class 9

## **HTML Forms**

HTML form is a section of the web page that contains controls like text input, password input, submit button, checkbox, radio button, menus ... , and we use them when we want to collect data from a user or a visitor.

```html 
<form action="server url" method="get|post">  
  textfield, textarea, radiobutton, button  ....
</form>  
```

### **HTML FORM TAGS**

| Tag | Description | 
| ---            | :--        |   
| `<form>` |   defines an HTML form to enter inputs by the used side.|  
| `<input>` |   defines an input control. |  
| `<textarea>` |   defines a multi-line input control. |  
| `<label>` |   defines a label for an input element. |  
| `<fieldset>` |   groups the related element in a form.|
| `<legend>` |   defines a caption for a `<fieldset>` element.  |
| `<select>` |   defines a drop-down list.  |
| `<optgroup>` |   defines a group of related options in a drop-down list. |
| `<option>` |   defines an option in a drop-down list. |
| `<button>` |   defines a clickable button. |
| `<datalist>` |  specifies a list of pre-defined options for input control. |
| `<keygen>` |   defines a key-pair generator field for forms. |
| `<output>` |   defines the result of a calculation. |


> Full Example

```html
<form action="./js/app.jsp">  
<table>  
<tr>  
    <td class="tdLabel"><label for="register_name" class="label">Enter name:</label></td>  
    <td><input type="text" name="name" value="" id="register_name" style="width:160px"/></td>  
</tr>  
<tr>  
    <td class="tdLabel"><label for="register_password" class="label">Enter password:</label></td>  
    <td><input type="password" name="password" id="register_password" style="width:160px"/></td>  
</tr>  
<tr>  
    <td class="tdLabel"><label for="register_email" class="label">Enter Email:</label></td>  
    <td  
><input type="email" name="email" value="" id="register_email" style="width:160px"/></td>  
</tr>  
<tr>  
    <td class="tdLabel"><label for="register_gender" class="label">Enter Gender:</label></td>  
    <td>  
<input type="radio" name="gender" id="register_gendermale" value="male"/>  
<label for="register_gendermale">male</label>  
<input type="radio" name="gender" id="register_genderfemale" value="female"/>  
<label for="register_genderfemale">female</label>  
    </td>  
</tr>  
<tr>  
    <td class="tdLabel"><label for="register_country" class="label">Select Country:</label></td>  
    <td><select name="country" id="register_country" style="width:160px">  
    <option value="Jordan">Jordan</option>  
    <option value="Palestine">Palestine</option>  
    <option value="UAE">UAE</option>  
</select>  
</td>  
</tr>  
<tr>  
    <td colspan="2"><div align="right"><input type="submit" id="register_0" value="register"/>  
</div></td>  
</tr>  
</table>  
</form>  
```

**the output**
>![forinatable](https://i.imgur.com/erD7SV5.png)

---


## **JS EVENTS**

> HTML events are `things` that happen to HTML elements. When JavaScript is used in HTML pages, JavaScript can `react` on these events.  <small> "w3 schools" <small>

**example**

```html
<h1 onclick="this.innerHTML = 'Hi this is a Heading!'">Click Here!</h1>
```

### **HTML Events attributes**

* Onload - onunload

they are events and triggered when the user enters or leaves the page.

The `onload` event used to check the browser type and browser version and load the a version of a web page based on the information.

```html
<body onload="checkloginstatus())">
```
* onchange

is often used in combination with validation of input fields.

```html
<input type="text" id="lastname" onchange="lowerCase()">
```

- see the following table for all html 5 js events
>![forinatable](https://i.imgur.com/SBDneXN.png)



[**Back**](https://odehabuzaid.github.io/reading-notes/)                     | [**TOP**](#Class-9) |

