# Active Slider
Slider for CSS masters.

- **The Active Class** - Active-Slider has one job, adding an "active" class for your desired HTML tags.
- **Keep your HTML beautiful** - Active Slider will not inject HTML, CSS or JS code.
- **Full control** - As a CSS master, you'll have full control over your slider with no injected Html or Css.

There is one rule, slides group must have the same number of elements.
For example: slide-images must have the same number of bullets elements.


## NPM

```
npm install active-slider
```

```javascript
import ActiveSlider from 'active-slider';

new ActiveSlider({
    sliderWrapper: '.slider-wrapper', 
    activeElements: ['.slide-image', '.bullet'],
}); 

```

## Parameters
- sliderWrapper
(string)(required) - Select the slider wrapper element.
Example: '.slider'
    
- activeElements
(array|string)(required) - Select elements to add the active class.
Example: ['.slide-image', '.bullet']
    
- swipeArea
(string)(optional) - Select the element that will be the swipe area.
Example: '.slide-images-container'

- clickableElements
(array|string)(optional) -  Add the active class to the clicked slide.
Example: '.bullet'

- prevNextButtons
(array)(optional) - Select the previous and next buttons.
Example: ['.prev', '.next']

- autoSlide
(number|boolean)(optional)  - Default time between slides is 3500 milliseconds. set to false if no need an auto slide.
Default: 3500

- stopAutoSlideOnClick
(array)(optional) - Select the elements to be the listeners for the click event in order to stop the auto slide.
Example: ['.prev', '.next']

- loop
(boolean)(optional) - Loop slider.
Default: true

- activeFirstSlide
(boolean)(optional) - Set to false in order to remove the active class from the first slide as default.
Default: true

## Example
https://codepen.io/guycohen85/pen/GRJoxvw
