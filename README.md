
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Video Icon Controlled by Buttons</title>
  <style>
    /* Make video look like an icon */
    #myVideo {
      width: 120px;
      height: 90px;
      display: block;
      margin-top: 20px;
      pointer-events: none; /* disables user interaction */
    }
  </style>
</head>
<body>
  <h1>Welcome to My GitHub Page</h1>

  <button onclick="playVideo()">Play</button>
  <button onclick="stopVideo()">Stop</button>

  <!-- Muted, small video -->
  <video id="myVideo" muted loop>
    <source src="Crystal Castles - KEROSENE (Lyrics).mp4" type="video/mp4">
    Your browser does not support the video tag.
  </video>

  <script>
    const video = document.getElementById("myVideo");

    function playVideo() {
      video.play();
    }

    function stopVideo() {
      video.pause();
      video.currentTime = 0;
    }
  </script>
</body>
</html>
