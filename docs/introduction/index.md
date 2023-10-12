<!DOCTYPE html>
<html>
<head>
  <style>
    #cube-container {
      perspective: 1200px;
      width: 200px;
      height: 200px;
    }
    
    #cube {
      position: relative;
      width: 100%;
      transform-style: preserve-3d;
      animation: rotate 5s linear infinite;
    }
    
    .face {
      position: absolute;
      width: 200px;
      height: 200px;
      background: #3498db;
      border: 2px solid #2980b9;
      text-align: center;
      line-height: 200px;
      font-size: 24px;
      font-weight: bold;
      color: white;
    }
    
    .face:nth-child(1) { transform: rotateY(0deg) translateZ(100px); }
    .face:nth-child(2) { transform: rotateY(90deg) translateZ(100px); }
    .face:nth-child(3) { transform: rotateY(180deg) translateZ(100px); }
    .face:nth-child(4) { transform: rotateY(-90deg) translateZ(100px); }
    .face:nth-child(5) { transform: rotateX(90deg) translateZ(100px); }
    .face:nth-child(6) { transform: rotateX(-90deg) translateZ(100px); }
    
    @keyframes rotate {
      0% { transform: rotateY(0deg); }
      100% { transform: rotateY(360deg); }
    }
  </style>
</head>
<body>
  <div id="cube-container">
    <div id="cube">
      <div class="face">Niko</div>
      <div class="face">IS</div>
      <div class="face">GOD</div>
      <div class="face">NIKO</div>
      <div class="face">IS</div>
      <div class="face">GOD</div>
    </div>
  </div>
</body>
</html>

