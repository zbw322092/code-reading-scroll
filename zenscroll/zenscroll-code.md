# zenscroll code reading

[1]
``` javascript
var getDocY = function () { return window.scrollY || docElem.scrollTop }
```
Get the vertical position in pixel; <br>

[2]
``` javascript
getTopOf: function (elem) { return elem.getBoundingClientRect().top + getDocY() - docElem.offsetTop }
```