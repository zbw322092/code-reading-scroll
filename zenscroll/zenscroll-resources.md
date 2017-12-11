# zenscroll related resources
## scroll-behavior
[1] scroll-behavior
https://css-tricks.com/almanac/properties/s/scroll-behavior/ <br>

[2] Smooth Scrolling
https://css-tricks.com/snippets/jquery/smooth-scrolling/ <br>

[3] smooth scroll polyfill
http://iamdustan.com/smoothscroll/ <br>

[4] scroll-behavior MDN
https://developer.mozilla.org/en-US/docs/Web/CSS/scroll-behavior <br>

`scroll-behavior` is not support in `Safari` and `IE`(including `Edge`);
Details: https://developer.mozilla.org/en-US/docs/Web/CSS/scroll-behavior#Browser_compatibility <br>

todo
[1] Smooth Scrolling and Accessibility
https://css-tricks.com/smooth-scrolling-accessibility/ <br>

## Document.scrollingElement MDN
https://developer.mozilla.org/en-US/docs/Web/API/Document/scrollingElement <br>

The `scrollingElement` read-only property of the `Document` interface returns a reference to the `Element` that **scrolls the document**. In **standards mode**, this is the root element of the document, **`document.documentElement`**.

When in **quirks mode**, the `scrollingElement` attribute returns the **HTML body element** (or null if it does not exist).

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

## Document.documentElement
https://developer.mozilla.org/en-US/docs/Web/API/Document/documentElement <br>

> `Document.documentElement` returns the `Element` that is the **root element** of the document (for example, the <html> element for HTML documents).


## Get an Element's Position Using JavaScript
https://www.kirupa.com/html5/get_element_position_using_javascript.htm <br>

## Performance - Date.now() vs Date.getTime()
https://stackoverflow.com/a/12517413/6498272 <br>

> ... the time value from any already-created Date instance is frozen at the time of its construction

## Element.scrollHeight
https://developer.mozilla.org/en-US/docs/Web/API/Element/scrollHeight <br>

> The `Element.scrollHeight` read-only property is a measurement of the height of an element's content, **including content not visible** on the screen due to overflow.

> The `scrollHeight` value is equal to the minimum height the element would require in order to fit all the content in the viewport without using a vertical scrollbar. It **includes the element's padding, but not its border or margin.** It can also include the height of pseudo-elements such as `:before` or `:after`.

<br>
<br>
<br>
<br>

## -------------------------------------------
## Browser History API
### Using the HTML5 History API
https://css-tricks.com/using-the-html5-history-api/ <br>
`history.replaceState`, `history.pushState`, `popstate` and so forth.

### Manipulating the browser history MDN
https://developer.mozilla.org/en-US/docs/Web/API/History_API <br>

### Getting Started With The History API
http://blog.teamtreehouse.com/getting-started-with-the-history-api <br>

Try the example in this post. <br>

### History API: Scroll Restoration
https://developers.google.com/web/updates/2015/09/history-api-scroll-restoration <br>


### todo
[1] Implementing pushState for twitter.com
https://blog.twitter.com/engineering/en_us/a/2012/implementing-pushstate-for-twittercom.html <br>

[2] Making AJAX applications crawlable
https://developers.google.com/webmasters/ajax-crawling/docs/learn-more <br>
