jQuery-Marquee
==============

jQuery plugin to scroll the text like the old traditional marquee

Update:
-------
 - The plugin is improved to adjust the speed according to the lenth of the text automatically. For more details read: https://github.com/aamirafridi/jQuery.Marquee/issues/1
 - 'duplicated' option added. See the details below in Options section.

**Blog post:** http://aamirafridi.com/jquery/jquery-marquee-plugin

Options:
--------
 - **speed:** Speed in milliseconds of the marquee. Please make note that same speed value will react differently for text with different lengths. Default is 10000.
 - **gap:** Gap in pixels between the tickers. Default is 20.
 - **delayBeforeStart:** Time in milliseconds before the marquee starts animating. Default is 1000
 - **direction:** Direction towards which the marquee will animate 'left' or 'right'. Default is 'left'.
 - **duplicated:** true or false - should the marquee be duplicated to show an effect of continues flow. Default is false.

Demo:
-----
 - http://jquery.aamirafridi.com/jquerymarquee/

Use:
----

###HTML:

```html
<div class='marquee'>Lorem ipsum dolor sit amet, consectetur adipiscing elit END.</div>
```

###CSS:
```css
.marquee {
  width: 300px; /* the plugin works for responsive layouts so if width is not necessary */
  overflow: hidden;
  border:1px solid #ccc;
}
```

###Apply plugin:
```javascript
/**
 * Example of starting a plugin with options.
 * I am just passing all the default options
 * so you can just start the plugin using $('.marquee').marquee();
*/
$('.marquee').marquee({
	//speed in milliseconds of the marquee
	speed: 15000,
	//gap in pixels between the tickers
	gap: 50,
	//time in milliseconds before the marquee will start animating
	delayBeforeStart: 0,
	//'left' or 'right'
	direction: 'left'
});
```
