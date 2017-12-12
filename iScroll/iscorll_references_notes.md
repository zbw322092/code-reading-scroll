# IScorll References Notes
## event.type
Event reference
event.type full list avaliable in MDN
https://developer.mozilla.org/en-US/docs/Web/Events

Some common DOM event types:
https://www.khanacademy.org/computing/computer-programming/html-css-js/html-js-dom-events/a/dom-event-types
> **mouse events** (`MouseEvent`): mousedown, mouseup, click, dblclick, mousemove, mouseover, mousewheel, mouseout, contextmenu<br/>
**touch events** (`TouchEvent`): touchstart, touchmove, touchend, touchcancel<br/>
**keyboard events** (`KeyboardEvent`): keydown, keypress, keyup<br/>
**form events**: focus, blur, change, submit<br/>
**window events**: scroll, resize, hashchange, load, unload

## MouseEvent.button
https://developer.mozilla.org/en-US/docs/Web/API/MouseEvent/button

The MouseEvent.button read-only property indicates which button was pressed on the mouse to trigger the event.

> A number representing a given button:
0: Main button pressed, usually the left button or the un-initialized state
1: Auxiliary button pressed, usually the wheel button or the middle button (if present)
2: Secondary button pressed, usually the right button
3: Fourth button, typically the Browser Back button
4: Fifth button, typically the Browser Forward button

## MouseEvent.pageX
https://developer.mozilla.org/en-US/docs/Web/API/MouseEvent/pageX

> The pageX read-only property of the MouseEvent interface returns the X (horizontal) coordinate in pixels of the event relative to the whole document. This property takes into account any horizontal scrolling of the page. 

Also, `MouseEvent.pageY`
https://developer.mozilla.org/en-US/docs/Web/API/MouseEvent/pageY

## HTMLElement.offsetWidth
https://developer.mozilla.org/en-US/docs/Web/API/HTMLElement/offsetWidth <br>

> The `HTMLElement.offsetWidth` read-only property returns the layout width of an element. Typically, an element's `offsetWidth` is a measurement which includes the **element borders, the element horizontal padding, the element vertical scrollbar (if present, if rendered) and the element CSS width**.


![offsetWidth](https://mdn.mozillademos.org/files/347/Dimensions-offset.png)

## HTMLElement.offsetHeight
https://developer.mozilla.org/en-US/docs/Web/API/HTMLElement/offsetHeight <br>

> The `HTMLElement.offsetHeight` read-only property is the height of the element including vertical padding and borders, as an integer.
Typically, an element's `offsetHeight` is a measurement in pixels of the **element's CSS height, including border, padding and the element's horizontal scrollbar (if present, if rendered).** It does not include the height of pseudo-elements such as :before or :after.

Both `HTMLElement.offsetWidth` and `HTMLElement.offsetHeight` value is round to integer. If you need a fractional value, use `element.getBoundingClientRect()`.

![offsetHeight](https://mdn.mozillademos.org/files/347/Dimensions-offset.png)


## todo
### Force reflow
[1] What forces layout / reflow
https://gist.github.com/paulirish/5d52fb081b3570c81e3a <br>

[2] ON LAYOUT & WEB PERFORMANCE
http://kellegous.com/j/2013/01/26/layout-performance/ <br>

[3] css triggers
https://csstriggers.com/ <br>



