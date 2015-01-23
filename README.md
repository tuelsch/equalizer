# equalizer

Set equal heights to your rows.


#### Prerequisites
- jQuery
- A container containing elements sharing the same width


#### Features
- Calculates and sets same height for all elements per row
- Waits for images to load and recalculates afterwards


#### Installation
Download the script from this page and include the following script tag just after the closing `</body` tag, or you know, use some browserify magic to bundle it with your other scripts.
```
<script src="/path/to/equalizer.min.js"></script>
```
Bower support is going to happen soon, in the meantime you can install the package via
```
bower install maxomedia/equalizer --save
```


#### Options
```javascript
var options = {
  childSelector: '.child', // A jquery selector for the child containers
  updateEventName: 'resize'   // Which event you want to listen to (on $(window))
};
```


#### Functions
```javascript
$('.toBeEqualizedContainer').equalize(options); // Initialize the function
$('.toBeEqualizedContainer').equalizeAgain();   // Recalculate without initialization
```


#### Demo
See http://codepen.io/tuelsch/full/ogwLWX/ for a demo of the script.