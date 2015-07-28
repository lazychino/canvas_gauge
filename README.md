#canvasgauge.js

####NOTE: this project is not actively develop

This is a library I made originally to display sensor data on hardware projects. It can be use for anything you like and is written in pure Javascript. No dependencies!

Currently there only 2 types of gauges: needle gauge, and rectangle bar (horizontal movement),
I'm planning to make some more gauge types and enabled css to modify the gauges look.

[Here is a live demo](http://lazychino.github.io/canvas_gauge/)

#####usage:
```html 
<script src='canvasgauge.js'></script>
<canvas id="canvas_id" width="200" height="200"></canvas>
<script>
   // create gauge object
   var gauge2 = new Gauge('canvas_id', {options object});
   
   // update gauge image (gauge is not draw until this functios is call)
   gauge2.draw( value );        
</script>
```
#####options:
- color: foreground color
- bgColor: background color
- textColor: gauge text color (currently only for needle gauge)
- time: time gauge take to update to new value
- range: {
  min: lower bound value,
  max: upper bound value
}
- mode: gauge mode (default='bar', 'needle')


---


The MIT License (MIT)

Copyright (c) 2013-2015 Pedro A. Melendez
