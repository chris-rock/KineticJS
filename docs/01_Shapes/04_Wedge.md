To create a wedge with `KineticJS`, we can instantiate a `Kinetic.Wedge()` object.  For a full list of attributes and methods, check out the [Kinetic.Wedge documentation](http://kineticjs.com/docs/Kinetic.Wedge.html).

<iframe width="350" height="350" src="../Examples/Shapes/Wedge.html" frameborder="0" allowfullscreen></iframe>

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
        width: 300,
        height: 300
      });

      var layer = new Kinetic.Layer();

      var wedge = new Kinetic.Wedge({
        x: stage.getWidth() / 2,
        y: stage.getHeight() / 2,
        radius: 70,
        angleDeg: 60,
        fill: 'red',
        stroke: 'black',
        strokeWidth: 4,
        rotationDeg: -120
      });

      // add the shape to the layer
      layer.add(wedge);

      // add the layer to the stage
      stage.add(layer);
    </script>
  </body>
</html>

```