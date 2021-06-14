# Class 7

## **Domain Modeling**

Domain modeling is the process of creating a conceptual model in code for a specific problem. A model describes the various entities, their attributes and behaviors, as well as the constraints that govern the problem domain. 

An entity that stores data in properties and encapsulates behaviors in methods is commonly referred to as an object-oriented model.


[read More](https://github.com/codefellows/domain_modeling#domain-modeling)


**HTML Tables**

tables used to display data that make sense in spreadsheet software. They consist of rows and columns used on websites for the effective displaying of tabular data.
## Example

```html
<h2>HTML Table</h2>

<table>
  <tr>
    <th>Company</th>
    <th>Contact</th>
    <th>Country</th>
  </tr>
  <tr>
    <td>Alfreds Futterkiste</td>
    <td>Maria Anders</td>
    <td>Germany</td>
  </tr>
  <tr>
    <td>Centro comercial Moctezuma</td>
    <td>Francisco Chang</td>
    <td>Mexico</td>
  </tr>
  <tr>
    <td>Ernst Handel</td>
    <td>Roland Mendel</td>
    <td>Austria</td>
  </tr>
  <tr>
    <td>Island Trading</td>
    <td>Helen Bennett</td>
    <td>UK</td>
  </tr>
  <tr>
    <td>Laughing Bacchus Winecellars</td>
    <td>Yoshi Tannamuri</td>
    <td>Canada</td>
  </tr>
  <tr>
    <td>Magazzini Alimentari Riuniti</td>
    <td>Giovanni Rovelli</td>
    <td>Italy</td>
  </tr>
</table>
```

this code will produce 
>![Jsimg](https://i.imgur.com/wAk3Zh3.png)


**Object Constructors**

Sometimes we need a "blueprint" for creating many objects of the same "type". so we make an object constructor function.

example 

```js
function Person(Name, age, Isgraduate, gpa) {
  this.Name = Name;
  this.age = age;
  this.Isgraduate = Isgraduate;
  this.gpa = gpa;
}
```

and then we call the function above to create objects from the same type.

```js
const myFather = new Person("Odeh", "30", true, "good");
const myMother = new Person("sanad", "3", false, "NA");
```

[**Back**](https://odehabuzaid.github.io/reading-notes/)                     | [**TOP**](#Class-7) |