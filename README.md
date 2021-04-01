# SVG-CSS-Button-animated-stroke
.....html....
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width">
    <title>repl.it</title>
    <link href="style.css" rel="stylesheet" type="text/css" />
  </head>
  <body>
    
       <a class="cta">
  <svg>
    <rect x="0" y="0" fill="none" width="130" height="55" />
  </svg>
  HOVER Me
</a>
  </body>
</html>
.....css......
body {
  background: rgba(102, 180, 216, 0.062);
  text-align: center;
  padding-top: 70px;
}

.cta {
  position: relative;
  display: inline-block;
  margin-top: 15px;
  width: 130px;
  height: 55px;
  font-size: 14px;
  line-height: 55px;
  text-align: center;
  text-transform: uppercase;
  color: rgb(182, 36, 11);
  cursor: pointer;
  overflow: hidden;
}
.cta svg {
  position: absolute;
  top: 0;
  left: 0;
}
.cta svg rect {
  stroke: rgb(202, 10, 116);
  stroke-width: 3;
  stroke-dasharray: 322, 0;
  stroke-dashoffset: 0;
  transition: all 350ms ease-out;
}

.cta:hover {
  color: #231fe7;
}
.cta:hover svg rect {
  stroke: #0f0302;
  stroke-width: 5;
  stroke-dasharray: 110, 312;
  stroke-dashoffset: 227;
}

.cta:active {
  font-weight: 600;
}
