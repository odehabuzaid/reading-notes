# Class 12

## **CHARTS**

Charts are far better for displaying data visually than tables and have the added benefit that no one is ever going to press-gang them into use as a layout tool. They’re easier to look at and convey data quickly, but they’re not always easy to create.


To see how to use chart.js we’re going to create a set of 3 graphs; one will show the number of buyers a fictional product has over the course of 6 months, this will be a line chart; the second will show which countries the customers come from, this will be the pie chart; finally we’ll use a bar chart to show profit over the period.

```html
<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="utf-8" />
        <title>Chart.js demo</title>
        <script src='Chart.min.js'></script>
    </head>
    <body>
    </body>
</html>
```

**Drawing a pie chart**

Our line chart is complete, so let’s move on to our pie chart. First, we need the canvas element:

```html
<canvas id="countries" width="600" height="400"></canvas>
```

>> THE content 
```js
var countries= document.getElementById("countries").getContext("2d");
new Chart(countries).Pie(pieData, pieOptions);
```

>![Jsimg](https://miro.medium.com/max/3648/1*ZxZMc4n6XJxlNjA-p4WAKg.png)


[**Back**](https://odehabuzaid.github.io/reading-notes/)                     | [**TOP**](##CHARTS) |

