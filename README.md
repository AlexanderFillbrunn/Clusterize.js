# Clusterize.js
[![Clusterize.js on NPM](https://img.shields.io/npm/v/clusterize.js.svg)](https://www.npmjs.com/package/clusterize.js) 
[![Clusterize.js on Bower](https://img.shields.io/bower/v/clusterize.svg)](http://bower.io/search/?q=clusterize)
[![Package Quality](http://npm.packagequality.com/shield/clusterize.js.svg)](http://packagequality.com/#?package=clusterize.js)
[![Join the chat at https://gitter.im/NeXTs/Clusterize.js](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/NeXTs/Clusterize.js?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)

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

[Demo, usage, etc…](https://clusterize.js.org/)

[![example](http://nexts.github.io/Clusterize.js/img/table_example.gif)](https://clusterize.js.org/)
