#progre(c)ss


###Pure CSS progress bars with minimal effort


#### Usage
1. Include the [stylesheet](https://raw2.github.com/jh3y/progre-c-ss/master/progrecss.css).
2. Add the class `progrecss` to your element (any existing element)
3. Add a data attribute `data-progrecss` defining the completion percentage (1 to 100) and any optional data attributes and classes for your desired behaviour/position/appearance[*](#helpers)
4. Update progre(c)ss value if necessary using simple vanilla js or whatever suits you best!

That's it!

```html
    <div class="progrecss" data-progrecss="77">
		My first progre(c)ss!
	</div>
```

##### Browser Support

From what I can gather having a look at caniuse, progre(c)ss should be fully supported from IE10 up. This is purely because of transition, but if I remember rightly this can be shimmed.

##### Mocking progre(c)ss

You can easily mock progress by using the helper attributes and classes. Refer [here](#helpers).

##### Helpers

There are some helper classes and attributes you can add to help you out!

######positioning classes
* `top`(default)
	The default positioning for a progrecss bar is at the top of an element.
* `bottom`
	Positions the progrecss bar at the bottom of the element.
* `fixed`
	Gives a fixed position of `0,0` relative to the container of the element.

######color classes
* `green`(default)
* `blue`
* `red`
* `purple`
* `orange`
* `yellow`

######mocking attribute
* `data-progrecss-mock` - takes a number value that defines duration of how long the mocked progress should take in seconds (up to 120).

######mocking classes
* `mock` - required in order to initiate a mock.
* `staggered` - will stagger the mock halting at different percentages (can be customised by altering source files).

#### Development/Customisation

__progre(c)ss__ is developed with __less__/__sass__ /__scss__ making the actual amount of code written minimal in order to generate the stylesheet by making use of looping.

When using the __less__/__sass__/__scss__ file there are already some variables in place so you can roll out a new theme easily.

Those variables are:

* color
* height
* box-shadow
* opacity
* border-radius
* transition(-webkit-transition)

Also to edit things like the way in which a staggered mock progress behaves you can modify the existing keyframes in place.

#### Contributing

Any suggestions, improvements or issues are welcome. :)

@jh3y

#### License

MIT

Copyright (c) 2014 [@jh3y](https://github.com/jh3y)
