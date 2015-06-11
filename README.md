# jQuery scrollToTop

The powerful jQuery plugin that creates a button which provides a function to scroll to page top. <a href="http://amazingsurge.github.io/jquery-scrollToTop/">Project page and demos</a><br />
Download: <a href="https://github.com/amazingSurge/jquery-scrollToTop/archive/master.zip">jquery-scrollToTop-master.zip</a>

***

## Features


* **Lightweight size** — 1 kb gzipped

## Dependencies
* <a href="http://jquery.com/" target="_blank">jQuery 1.83+</a>

## Usage

Import this libraries:
* jQuery
* jquery-scrollToTop.js

And CSS:
* scrollToTop.css 


Create base html element:
```html
	<div class="container">
        <div>
            <h3>Css3/html5</h3>
            <p>Built-on CSS3 and HTML5 semantics to allow you to start captializing on a next generation standard.</p>
        </div>
	</div>
```

Initialize tabs:
```javascript
$('body').scrollToTop({skin: 'cycle', easing: 'easeInOutElastic'});
```

Or initialize tabs with custom settings:
```javascript
$("body").scrollToTop({
	namespace: 'scrollToTop',
	skin: null,
	speed: 1000,
	easing: 'linear',
	distance: 200,
	text: 'Scroll To Top',
	animation: 'fade',
	animationSpeed: 500
});
```

## Settings

```javascript
{   

	// Optional property, Set a namespace for css class
	namespace: 'scrollToTop',
	
	//Optional property, set transition effect, it works after you load specified skin file
    skin: 'null',

	//Optional property, set the trasition effect for the duration when scroll to top
    speed: 1000,

	//Optional property, set a class name
    easing: 'linear',

	//Optional property, if scrollTop greater than the value of distance, the scroll button will show 
    distance: 200,

    //Optional property, a tip message for the scroll button
    text: 'scroll To Top',

	//Optional property, set a class name
    animation: 'fade',

    //Optional property, set the trasition effect for the duration
    animationSpeed: 500
}
```

## Public methods

jquery scrollToTop has different methods , we can use it as below :
```javascript
// trigger the event of disable
$("body").scrollToTop("disable");

// trigger the event of enable
$("body").scrollToTop("enable");

// unbind all events
$("body").scrollToTop("destroy");

```

## Event / Callback

* <code>ScrollToTop::jump</code>: trigger when jump the page top
* <code>ScrollToTop::show</code>: trigger when the scrollTop greater than the value of distance
* <code>ScrollToTop::hide</code>: trigger when the scrollTop less than the value of distance
* <code>ScrollToTop::disable</code>: trigger when the element is disabled
* <code>ScrollToTop::enable</code>: trigger when the element is enabled

how to use event:
```javascript
$(document).on('ScrollToTop::jump', function(event,instance) {
    // instance means current scrollToTop instance 
    // some stuff
});
```

## Browser support
jquery-scrollToTop is verified to work in Internet Explorer 7+, Firefox 2+, Opera 9+, Google Chrome and Safari browsers. Should also work in many others.

Mobile browsers (like Opera mini, Chrome mobile, Safari mobile, Android browser and others) is coming soon.

## Changes

| Version | Notes                                                            |
|---------|------------------------------------------------------------------|
|     ... | ...                                                              |


## Author
[amazingSurge](http://amazingSurge.com)

## License
jQuery-scrollToTop plugin is released under the <a href="https://github.com/amazingSurge/jquery-scrollToTop/blob/master/LICENCE.GPL" target="_blank">GPL licence</a>.


