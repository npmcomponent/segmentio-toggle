*This repository is a mirror of the [component](http://component.io) module [segmentio/toggle](http://github.com/segmentio/toggle). It has been modified to work with NPM+Browserify. You can install it using the command `npm install npmcomponent/segmentio-toggle`. Please do not open issues or send pull requests against this repo. If you have issues with this repo, report it to [npmcomponent](https://github.com/airportyh/npmcomponent).*
# toggle

  A toggle UI element.
  
  ![on](https://i.cloudup.com/kjeyaT5oFH.png)
  ![off](https://i.cloudup.com/hEd5319GKt.png)

## Installation

    $ component install segmentio/toggle

## Example
    
```js
var Toggle = require('toggle');

var toggle = new Toggle();
document.body.appendChild(toggle.el);

toggle.value(); // false

toggle.value(true);
toggle.value(); // true

toggle.toggle();
toggle.value(); // false
```

## API

### Toggle(value, el)
  Create a new toggle with an optional starting `value` and optional `el` to use instead of creating one.

### #el
  The toggle's DOM element.

```html
<div class="toggle">
  <label class="toggle-on-label"></label>
  <div class="toggle-switch">
    <input class="toggle-checkbox" type="checkbox">
  </div>
  <label class="toggle-off-label"></label>
</div>
```

### #value(val)
  Get or set the value of the toggle.

### #name(name)
  Set the toggle's internal checkbox's name, so forms can be submitted properly.

### #toggle()
  Toggle the value of the toggle.

### #label(on, off)
  Set the on and off labels's HTML.

### #addClass(name)
  Add a class to the toggle's element.

### #removeClass(name)
  Remove a class from the toggle's element.

## License

  MIT
