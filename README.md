# jQuery scrollToTop

The powerful jQuery plugin that creates a button help you  scroll to page's top. <a href="http://amazingsurge.github.io/jquery-scrollToTop/">Project page and demos</a><br />
Download: <a href="https://github.com/amazingSurge/jquery-scrollToTop/archive/master.zip">jquery-scrollToTop-master.zip</a>

***

## Features

* **The plugin supports relative animations**
* **The call to the plugin can be made in 2 different ways** — $().scrollTo( target, duration, settings ) or $().scrollTo( target, settings ). 
* **Lightweight size** — 1 kb gzipped
## Dependencies
* <a href="http://jquery.com/" target="_blank">jQuery 1.83+</a>

## Usage

Import this libraries:
* jQuery
* jquery-scrollToTop.min.js

And CSS:
* jquery-scrollToTop.css - desirable if you have not yet connected one

Initialize scrollToTop:
```javascript
$('body').scrollToTop();
```

Or initialize scrollToTop with custom settings:
```javascript
$('body').scrollToTop({
     speed: 1000,
     easing: 'linear',
	 distance: 200,
	 text: 'Scroll To Top',
	 animation: 'fade', // fade, slide, none
	 animationSpeed: 500,
	 skin: null,
	 namespace: 'scrollToTop'
});
```



## Settings

```javascript
{
    // Optional property, set the speed scroll to page's top
    speed: 1000,

    //Optional property, set easing type
    easing: 'linear', 

    //Optional property, Distance from top before showing element (px)
    distance: 200,

    //Optional property, Text for element, can contain HTML
    text: 'Scroll To Top',

    //Optional property, set the type of animation ,options: fade slide none
    animation: 'fade',

    //Optional property, set animation speed
    animationSpeed: 500,

    //Optional property,  choose element's skin, more skins is coming soon
    skin: null,

    //Optional property,  Set a namespace for css class
    namespace: 'scrollToTop'
      
}
```

## Public methods

jquery scrollToTop has different methods , we can use it as below :
```javascript
// page will scroll to top
$('body').scrollToTop("jump");

// the plugin's function become disable
$('body').scrollToTop("disable");

// the plugin's function become enable
$('body').scrollToTop("enable");

//  remove Dom emement and unbound all events 
$('body').scrollToTop("destroy");


## Browser support
jquery-scrollToTop is verified to work in Internet Explorer 7+, Firefox 2+, Opera 9+, Google Chrome and Safari browsers. Should also work in many others.

Mobile browsers (like Opera mini, Chrome mobile, Safari mobile, Android browser and others) is coming soon.
```

## Changes

| Version | Notes                                                            |
|---------|------------------------------------------------------------------|
|     ... | ...                                                              |


## Author
[amazingSurge](http://amazingSurge.com)

## License
jQuery-scrollToTop plugin is released under the <a href="https://github.com/amazingSurge/jquery-scrollToTop/blob/master/LICENCE.GPL" target="_blank">GPL licence</a>.


