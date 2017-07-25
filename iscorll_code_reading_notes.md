# Code Reading
`utils` 1-322
`IScroll` 323-420
`IScroll.prototype` 422-1833
`Indicator.prototype` 1835-2193


## Init Phase

initial `myScorll`:
``` javascript
directionX:0 // default value
directionY:0 // default value
enabled:true
endTime:0 // default value in IScroll.prototype this.endTime = 0;
hasHorizontalScroll:undefined
hasVerticalScroll:true
isInTransition:false
maxScrollX:0
maxScrollY:-1432
options:Object
scroller:div#scroller
scrollerHeight:2000
scrollerStyle:CSSStyleDeclaration
scrollerWidth:160
translateZ:" translateZ(0)"
wrapper:div#wrapper
wrapperHeight:568
wrapperOffset:Object
wrapperWidth:160
x:0
y:0
_events:Object
```

initial `myScroll.constructor.prototype`:
``` javascript
destroy:function ()
disable:function ()
enable:function ()
getComputedPosition:function ()
goToPage:function (x, y, time, easing)
handleEvent:function (e)
next:function (time, easing)
off:function (type, fn)
on:function (type, fn)
prev:function (time, easing)
refresh:function ()
resetPosition:function (time)
scrollBy:function (x, y, time, easing)
scrollTo:function (x, y, time, easing)
scrollToElement:function (el, time, offsetX, offsetY, easing)
version:"5.2.0-snapshot"
_animate:function (destX, destY, duration, easingFn)
_end:function (e)
_execEvent:function (type)
_init:function ()
_initEvents:function (remove)
_initIndicators:function ()
_initKeys:function (e)
_initSnap:function ()
_initWheel:function ()
_key:function (e)
_move:function (e)
_nearestSnap:function (x, y)
_resize:function ()
_start:function (e)
_transitionEnd:function (e)
_transitionTime:function (time)
_transitionTimingFunction:function (easing)
_translate:function (x, y)
_wheel:function (e)
```

when an `IScroll` instance is created, follwing properties will be created:
``` javascript
this.wrapper = typeof el == 'string' ? document.querySelector(el) : el;
this.scroller = this.wrapper.children[0];
this.scrollerStyle = this.scroller.style;	
```

`IScroll this.options`:
``` javascript
	this.options = {

		resizeScrollbars: true,

		mouseWheelSpeed: 20,

		snapThreshold: 0.334,

// INSERT POINT: OPTIONS
		disablePointer : !utils.hasPointer,
		disableTouch : utils.hasPointer || !utils.hasTouch,
		disableMouse : utils.hasPointer || utils.hasTouch,
		startX: 0,
		startY: 0,
		scrollY: true,
		directionLockThreshold: 5,
		momentum: true,

		bounce: true,
		bounceTime: 600,
		bounceEasing: '',

		preventDefault: true,
		preventDefaultException: { tagName: /^(INPUT|TEXTAREA|BUTTON|SELECT)$/ },

		HWCompositing: true,
		useTransition: true,
		useTransform: true,
		bindToWrapper: typeof window.onmousedown === "undefined"
	};
```

when an `IScroll` instance is created, follwing functions will be executed:
``` javascript
	this._init();
	this.refresh();

	this.scrollTo(this.options.startX, this.options.startY);
	this.enable();
```


### this._init()
`this._init()` calls `_initEvents`. `_initEvents` register events on several target objects.

Then in `this._init()`, calls `this._initIndicators()`, `this._initWheel()`, `this._initSnap()` and `this._initKeys()` according to specified options.

`this._initWheel` register wheel events.

`this._initSnap` enable iScroll snap to fixed positions and elements.
When `snap` is enabled, method like `goToPage`, `next` and `prev` can be called.


### this.refresh()
In this method, set: 
`this.wrapperWidth`, `this.wrapperHeight`
`this.scrollerWidth`, `this.scrollerHeight`
`this.maxScrollX`, `this.maxScrollY`
`this.hasHorizontalScroll`, `this.hasVerticalScroll`
`this.endTime`, 
`this.directionX`, `this.directionY`
`this.wrapperOffset`

### this.scrollTo
scroll to any position with `scrollTo` method.

In `scrollTo`, some 'internal methods'(with `_`  before its name) `_transitionTimingFunction`, `_transitionTime`, `_translate`, `_animate` will be called.


### other initial values
Other initial values are clearly explained in [API DOC]((https://github.com/cubiq/iscroll) ). Reference it when browse code.


