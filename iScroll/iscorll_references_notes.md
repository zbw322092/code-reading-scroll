# IScorll References Notes
1. event.type
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

2. MouseEvent.button
https://developer.mozilla.org/en-US/docs/Web/API/MouseEvent/button

The MouseEvent.button read-only property indicates which button was pressed on the mouse to trigger the event.

> A number representing a given button:
0: Main button pressed, usually the left button or the un-initialized state
1: Auxiliary button pressed, usually the wheel button or the middle button (if present)
2: Secondary button pressed, usually the right button
3: Fourth button, typically the Browser Back button
4: Fifth button, typically the Browser Forward button

3. MouseEvent.pageX
https://developer.mozilla.org/en-US/docs/Web/API/MouseEvent/pageX

> The pageX read-only property of the MouseEvent interface returns the X (horizontal) coordinate in pixels of the event relative to the whole document. This property takes into account any horizontal scrolling of the page. 

Also, `MouseEvent.pageY`
https://developer.mozilla.org/en-US/docs/Web/API/MouseEvent/pageY