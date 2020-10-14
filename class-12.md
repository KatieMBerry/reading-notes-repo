//// Chart.js API ////
- uses HTML5 canvas ele to draw the graph to the page
 <!-- <script src='Chart.min.js'></script> -->
    - foot of the body will house another script tag that retrieves the context, and put data within:
        FOR A LINE CHART
        <!-- - body > <canvas id="buyers" width="600" height="400"></canvas>
        - foot of body > <script>
                            var buyers = document.getElementById('buyers').getContext('2d');
                            new Chart(buyers).Line(buyerData);
                            var buyerData = {
                                labels : ["January","February","March","April","May","June"],
                                datasets : [
                                    {
                                        fillColor : "rgba(172,194,132,0.4)",
                                        strokeColor : "#ACC26D",
                                        pointColor : "#fff",
                                        pointStrokeColor : "#9DB86D",
                                        data : [203,156,99,251,305,247]
                                    }
                                ]
                         </script> -->
        PIE CHART
        <!-- - foot of body > <script>
                            var countries= document.getElementById("countries").getContext("2d");
                            new Chart(countries).Pie(pieData, pieOptions);
                            var pieData = [
                                    {
                                        value: 20,
                                        color:"#878BB6"
                                    },
                                    {
                                        value : 40,
                                        color : "#4ACAB4"
                                    },
                                    {
                                        value : 10,
                                        color : "#FF8153"
                                    },
                                    {
                                        value : 30,
                                        color : "#FFEA88"
                                    }
                                ];
                            var pieOptions = {
                                segmentShowStroke : false,
                                animateScale : true
                                }
                            </script> -->
        BAR CHART
        <!-- foot of body > <script>    
                                var income = document.getElementById("income").getContext("2d");
                                new Chart(income).Bar(barData);
                                var barData = {
                                    labels : ["January","February","March","April","May","June"],
                                    datasets : [
                                        {
                                            fillColor : "#48A497",
                                            strokeColor : "#48A4D1",
                                            data : [456,479,324,569,702,600]
                                        },
                                        {
                                            fillColor : "rgba(73,188,170,0.4)",
                                            strokeColor : "rgba(72,174,209,0.4)",
                                            data : [364,504,605,400,345,320]
                                        }

                                    ]
                                }
                            </script> -->

//// Basic Usage of Canvas ////
- canvas ele has only width & height attributes (optional - can also be set w/ DOM) - don't use CSS for this
    - default will be 300w 150h
    - can use fallback content for older browsers
- 2D rendering context: uses method getContext() - takes in type of context (2d vs 3d)

//// Drawing Shapes ////
- grid default: 1 unit = 1px on canvas
    - origin of grid = top-left corner (0, 0) and all eles placed relative to this
- rectangles, where w/h are size of rectangle: 
    1. fillRect(x, y, width, height) = Draws a filled rectangle
    2. strokeRect(x, y, width, height) = Draws a rectangular outline
    3. clearRect(x, y, width, height) = Clears the specified rectangular area, making it fully transparent
- paths: a list of points connected by segments
    - to make shapes with paths:
        1. First, you create the path.
        2. Then you use drawing commands to draw into the path.
        3. Once the path has been created, you can stroke or fill the path to render it.
    - beginPath()
    - closePath()
    - stroke()
    - fill()
    - moveTo(x, y)
    - lineTo(x, y) = straight lines
    - arc/circles:
        - arc(x, y, radius, startAngle, endAngle, anticlockwise)
        - arcTo(x1, y1, x2, y2, radius)
    - Bezier/quadratic curves:
        - quadraticCurveTo(cp1x, cp1y, x, y) - has a start/end pointsw/one control point
        - bezierCurveTo(cp1x, cp1y, cp2x, cp2y, x, y) - has 2 cotrol points
- Path2D() - ?

//// Applying Styles & Colors ////
- fillStyle = color = Sets the style used when filling shapes
- strokeStyle = color = Sets the style for shapes' outlines.
- createPattern(image, type): 
    - repeat
    - no-repeat
    - repeat-x
    - repeat-y

//// Drawing Text ////
- fillText(text, x, y [, maxWidth]) = Fills a given text at the given (x,y) position. Optionally with a maximum width to draw.
- strokeText(text, x, y [, maxWidth]) = Strokes a given text at the given (x,y) position. Optionally with a maximum width to draw.

