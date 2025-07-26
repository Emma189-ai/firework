<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Happy Birthday</title>
  <style>
    body, html { margin:0; padding:0; overflow:hidden; background:#001d3d; height:100%; position:relative; }
    #canvas { width:100%; height:100%; display:block; }
    .message { position:absolute; top:30%; width:100%; text-align:center; font-size:3em; color:white; text-shadow:0 0 20px rgba(255,255,255,0.8); pointer-events:none; }
  </style>
</head>
<body>
  <canvas id="canvas"></canvas>
  <div class="message">Happy Birthday</div>
  <script src="https://cdn.jsdelivr.net/gh/tswaters/fireworks-canvas/dist/index.min.js"></script>
  <script>
    const container = document.body;
    const fireworks = new Fireworks(container, { 
      trace: 3, explosion: 5, brightness: 50, delay: { min: 10, max: 30 }
    });
    fireworks.start();
  </script>
</body>
</html>
