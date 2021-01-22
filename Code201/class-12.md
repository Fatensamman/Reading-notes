

# Docs for the HTML(canvas)Element & Chart.js
* All elements in canvas are placed relative to the origin (0,0).
*  Canvas only supports two primitive shapes: rectangles and paths (lists of points connected by lines).
* fillRect(x, y, width, height) : Draws a filled rectangle.
*  strokeRect(x, y, width, height) : Draws a rectangular outline.
*  clearRect(x, y, width, height) : Clears the specified rectangular area, making it fully transparent.
*  Path methods : Methods to set different paths for objects.
*  beginPath() : Creates a new path. Once created, future drawing commands are directed into the path and used to build the path up.
*   closePath() : Adds a straight line to the path, going to the start of the current sub-path.
*  stroke() : Draws the shape by stroking its outline.
*  fill() : Draws a solid shape by filling the path's content area.
*  moveTo(x, y) : Moves the pen to the coordinates specified by x and y.
*  lineTo(x, y) : Draws a line from the current drawing position to the position specified by x and y.
*  arc(x, y, radius, startAngle, endAngle, anticlockwise) : Draws an arc which is centered at (x, y) position with radius r starting at startAngle and ending at endAngle going in the given direction indicated by anticlockwise (defaulting to clockwise).
*  arcTo(x1, y1, x2, y2, radius) : Draws an arc with the given control points and radius, connected to the previous point by a straight line.
*  quadraticCurveTo(cp1x, cp1y, x, y) : Draws a quadratic Bézier curve from the current pen position to the end point specified by x and y, using the control point specified by cp1x and cp1y.
*  bezierCurveTo(cp1x, cp1y, cp2x, cp2y, x, y) : Draws a cubic Bézier curve from the current pen position to the end point specified by x and y, using the control points specified by (cp1x, cp1y) and (cp2x, cp2y).
*  rect(x, y, width, height) : Draws a rectangle whose top-left corner is specified by (x, y) with the specified width and height.
*  The Path2D() constructor returns a newly instantiated Path2D object, optionally with another path as an argument (creates a copy), or optionally with a string consisting of SVG path data.
*  Path2D.addPath(path [, transform]) : Adds a path to the current path with an optional transformation matrix.
*  fillStyle = color : Sets the style used when filling shapes.
*  strokeStyle = color : Sets the style for shapes' outlines.
* globalAlpha = transparencyValue : Applies the specified transparency value to all future shapes drawn on the canvas. 
*  The value must be between 0.0 (fully transparent) to 1.0 (fully opaque). This value is 1.0 (fully opaque) by default.
*  lineWidth = value : Sets the width of lines drawn in the future.
*  lineCap = type : Sets the appearance of the ends of lines.
*  lineJoin = type : Sets the appearance of the "corners" where lines meet.
*  miterLimit = value : Establishes a limit on the miter when two lines join at a sharp angle, to let you control how thick the junction becomes.
*  getLineDash() : Returns the current line dash pattern array containing an even number of non-negative numbers.
*  setLineDash(segments) : Sets the current line dash pattern.
*  lineDashOffset = value : Specifies where to start a dash array on a line.
*  butt : The ends of lines are squared off at the endpoints.
*  round : The ends of lines are rounded.
*  square : The ends of lines are squared off by adding a box with an equal width and half the height of the line's thickness.
*  The setLineDash method and the lineDashOffset property specify the dash pattern for lines.
*  createLinearGradient(x1, y1, x2, y2) : Creates a linear gradient object with a starting point of (x1, y1) and an end point of (x2, y2).
*  createRadialGradient(x1, y1, r1, x2, y2, r2) : Creates a radial gradient. The parameters represent two circles, one with its center at (x1, y1) and a radius of r1, and the other with its center at (x2, y2) with a radius of r2.
*  repeat : Tiles the image in both vertical and horizontal directions.
*  repeat-x : Tiles the image horizontally but not vertically.
*  repeat-y : Tiles the image vertically but not horizontally.
*  no-repeat : Doesn't tile the image. It's used only once.
*  shadowOffsetX = float : ndicates the horizontal distance the shadow should extend from the object. This value isn't affected by the transformation matrix. The default is 0.
*  shadowOffsetY = float : Indicates the vertical distance the shadow should extend from the object. This value isn't affected by the transformation matrix. The default is 0.
*  shadowBlur = float : Indicates the size of the blurring effect; this value doesn't correspond to a number of pixels and is not affected by the current transformation matrix. The default value is 0.
*  shadowColor = color : A standard CSS color value indicating the color of the shadow effect; by default, it is fully-transparent black.
*  fillText(text, x, y [, maxWidth]) : Fills a given text at the given (x,y) position. Optionally with a maximum width to draw.
*  strokeText(text, x, y [, maxWidth]) : Strokes a given text at the given (x,y) position. Optionally with a maximum width to draw.
*  font = value : The current text style being used when drawing text. This string uses the same syntax as the CSS font property. The default font is 10px sans-serif.
*  textAlign = value : Text alignment setting. Possible values: start, end, left, right or center.  The default value is start.
*  textBaseline = value : Baseline alignment setting. Possible values: top, hanging, middle, alphabetic, ideographic, bottom. The default value is alphabetic.
*  direction = value : Directionality. Possible values: ltr, rtl, inherit. The default value is inherit.
It's easy to get started with Chart.js. All that's required is the script included in your page along with a single <canvas> node to render the chart.


## Creating a Chart


It's easy to get started with Chart.js. All that's required is the script included in your page along with a single node to render the chart.
In this example, we create a bar chart for a single dataset and render that in our page. You can see all the ways to use Chart.js in the usage documentation.
 (Links to an external site.)
Contributing
Before submitting an issue or a pull request to the project, please take a moment to look over the contributing guidelines first.
For support using Chart.js, please post questions with the chartjs tag on Stack Overflow.
 (Links to an external site.)
License
Chart.js is available under the MIT license.4
 (Links to an external site.)
The < canvas> element
At first sight a looks like the  element, with the only clear difference being that it doesn't have the src and alt attributes. Indeed, the element has only two attributes, width and height. These are both optional and can also be set using DOM properties. When no width and height attributes are specified, the canvas will initially be 300 pixels wide and 150 pixels high. The element can be sized arbitrarily by CSS, but during rendering the image is scaled to fit its layout size: if the CSS sizing doesn't respect the ratio of the initial canvas, it will appear distorted.
The element differs from an  tag in that, like for , , or elements, it is easy to define some fallback content, to be displayed in older browsers not supporting it, like versions of Internet Explorer earlier than version 9 or textual browsers. You should always provide fallback content to be displayed by those browsers.
 (Links to an external site.)
Drawing shapes with canvas
* The grid
* Drawing rectangles
* Drawing paths
* Drawing a triangle
* Arcs
* Making combinations
* Path2D objects
* Using SVG paths
 (Links to an external site.)
Colors
Up until now we have only seen methods of the drawing context. If we want to apply colors to a shape, there are two important properties we can use: fill Style and stroke Style