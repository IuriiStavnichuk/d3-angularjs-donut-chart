##D3 driven animated and reusable donut chart wrapper into AngularJS directive - [live demo](http://iuriistavnichuk.github.io/d3-angularjs-donut-chart/).

### How to install
 + Copy `donutChart.js` wherever you want
 + Reference it in your index.html file
 + Reference the module in your app file :
     angular.module('MainWebApp', ['donutChart'])

### How to use
A pie chart is called using this syntax :

```html
<donut-chart path-to-json = "'json/donut-chart.json'"></donut-chart>
```

The pie chart directive attribute : `path-to-json`.

#### path-to-json
Your data must be an array. Depending whether you wan a pie/donut or a gauge, the array can contain at least two rows, or only one.

##### path-to-json
Your data must be a JSON object.
```js
{
    "Results":
        [
            {"Title":"Funds Received",
                "CurrencySymbol":"$",
                "Amount":106.52,
                "TotalAmount":400,
                "CurrencyAbbreviation":"USD",
                "Unit":null,
                "TimeInterval":"/month"
            }
        ]
}
```
