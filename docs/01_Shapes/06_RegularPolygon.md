To create a regular polygon with `KineticJS`, we can instantiate a `Kinetic.RegularPolygon()` object.  For a full list of attributes and methods, check out the [Kinetic.RegularPolygon documentation](http://kineticjs.com/docs/Kinetic.RegularPolygon.html).

<iframe width="650" height="350" src="../Examples/Shapes/RegularPolygon.html" frameborder="0" allowfullscreen></iframe>

```html
<!DOCTYPE HTML>
<html>
  <head>
    <style>
      body {
        margin: 0px;
        padding: 0px;
      }
    </style>
  </head>
  <body>
    <div id="container"></div>
    <script src="http://d3lp1msu2r81bx.cloudfront.net/kjs/js/lib/kinetic-v5.1.0.min.js"></script>
    <script defer="defer">
      var stage = new Kinetic.Stage({
        container: 'container',
        width: 600,
        height: 300
      });

      var layer = new Kinetic.Layer();

      var hexagon = new Kinetic.RegularPolygon({
        x: 100,
        y: 150,
        sides: 6,
        radius: 70,
        fill: 'red',
        stroke: 'black',
        strokeWidth: 4
      });

      layer.add(hexagon);

      // add the layer to the stage
      stage.add(layer);
    </script>
  </body>
</html>
```