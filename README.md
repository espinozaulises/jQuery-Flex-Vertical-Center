# jQuery Flex Vertical Center

This jQuery plugin provides an easy way to vertically center an element in its parent. Even if the parents height changes after resizing the browser window, in a fluid or responsive layout for example.


## Usage

Simply include this file in your project (after loading jQuery) like this:

`<script defer src="js/jquery.flexverticalcenter.js"></script>`

Then call the plugin on the element which needs to be vertically centered in it's parent.

```html
<script>
$(document).ready(function() {
	$('#element-to-be-centered').flexVerticalCenter();
});
</script>
```

This will take the parents height, the elements own height and calculate the distance the element should have from the parents top to be vertically centered. This value is applied to the top margin of the element by default.


## Options

You can pass one parameter to the plugin, which is the css attribute that the value should be set on. The default is 'margin-top', but you can pass any attribute you would like. Most probably 'padding-top' or 'top'.

```html
<script>
$(document).ready(function() {
	$('#element-to-be-centered').flexVerticalCenter('padding-top');
});
</script>
```


## Note

The initial code was more or less borrowed from the awesome FitText plugin. http://fittextjs.com/