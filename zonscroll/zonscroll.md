# zonscroll code reading
## scroll-behavior
[1] scroll-behavior
https://css-tricks.com/almanac/properties/s/scroll-behavior/ <br>

[2] Smooth Scrolling
https://css-tricks.com/snippets/jquery/smooth-scrolling/ <br>

[3] smooth scroll polyfill
http://iamdustan.com/smoothscroll/ <br>

[4] scroll-behavior MDN
https://developer.mozilla.org/en-US/docs/Web/CSS/scroll-behavior 

todo
[1] Smooth Scrolling and Accessibility
https://css-tricks.com/smooth-scrolling-accessibility/ <br>

## Document.scrollingElement MDN
https://developer.mozilla.org/en-US/docs/Web/API/Document/scrollingElement <br>

``` javascript
var scrollElm = document.scrollingElement;
scrollElm.scrollTop = 0;
```

polyfill:
https://github.com/mathiasbynens/document.scrollingElement <br>

## window.scroll & window.scrollTo
https://developer.mozilla.org/en-US/docs/Web/API/Window/scrollTo <br>

https://developer.mozilla.org/en-US/docs/Web/API/Window/scroll <br>

JavaScript window.scroll vs. window.scrollTo?
https://stackoverflow.com/a/1925688/6498272 <br>

## Window.scrollY Window.scrollX
https://developer.mozilla.org/en-US/docs/Web/API/Window/scrollY <br>

https://developer.mozilla.org/en-US/docs/Web/API/Window/scrollX <br>

Both are **read only** value <br>

## Element.scrollTop
https://developer.mozilla.org/en-US/docs/Web/API/Element/scrollTop <br>

> The `Element.scrollTop` property gets or sets the number of pixels that an element's content is **scrolled vertically**.

> An element's scrollTop value is a measurement of the distance from the **element's top** to its **topmost visible content**.

Understand it with example. <br>

## window.innerHeight & window.outerHeright
https://developer.mozilla.org/en-US/docs/Web/API/Window/innerHeight <br>

![innerHeight vs innerHeight](https://mdn.mozillademos.org/files/443/FirefoxInnerVsOuterHeight2.png)

## Element.clientHeight
https://developer.mozilla.org/en-US/docs/Web/API/Element/clientHeight <br>

> clientHeight can be calculated as **CSS height + CSS padding - height of horizontal scrollbar (if present)**.

![Element.clientHeight](https://mdn.mozillademos.org/files/346/Dimensions-client.png)

## Element.getBoundingClientRect()

> The Element.getBoundingClientRect() method returns the size of an element and its position relative to the viewport.

> The result is the **smallest rectangle** which contains the **entire element**, with read-only `left`, `top`, `right`, `bottom`, `x`, `y`, `width`, and `height` properties describing the overall border-box in pixels. Properties other than `width` and `height` are **relative to the top-left of the viewport**.

## HTMLElement.offsetParent & HTMLElement.offsetTop
https://developer.mozilla.org/en-US/docs/Web/API/HTMLelement/offsetParent <br>

https://developer.mozilla.org/en-US/docs/Web/API/HTMLElement/offsetTop <br>

Simple but not exact explanation about `HTMLElement.offsetParent`
https://stackoverflow.com/a/17975012/6498272 <br>

Understand it with examples. <br>