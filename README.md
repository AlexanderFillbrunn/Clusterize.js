> Tiny vanilla JS plugin to display large data sets easily

This fork adds support for a function supplying html code for new rows.

**Usage:**
```javascript
// JavaScript
var clusterize = new Clusterize({
    rows: function(i) {
        return '<tr>' + Math.sqrt(i) + '</tr>'
    },
    // You need to specify the size because clusterize cannot determine it from the function
    size : 500000,
    scrollId: 'scrollArea',
    contentId: 'contentArea'
});
```
You can also still just pass an array instead of the function and the size

---

[Demo, usage, etc… (of the original library)](https://clusterize.js.org/)

[![example](http://nexts.github.io/Clusterize.js/img/table_example.gif)](https://clusterize.js.org/)
