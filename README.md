
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Play Audio + Muted Video Icon</title>
  <style>
    #myVideo {
      width: 120px;
      height: 90px;
      display: block;
      margin-top: 20px;
      pointer-events: none; /* Prevents user from clicking */
    }
  </style>
</head>
<body>
  <h1>Welcome to My GitHub Page</h1>

  <button onclick="playMedia()">Play</button>
  <button onclick="stopMedia()">Stop</button>

  <!-- Muted Video -->
  <video id="myVideo" muted loop>
    <source src="Crystal Castles - KEROSENE (Lyrics).mp4" type="video/mp4">
    Your browser does not support the video tag.
  </video>

  <!-- Playable Audio -->
  <audio id="myAudio">
    <source src="Crystal Castles KEROSENE Official.mp3" type="audio/mpeg">
    Your browser does not support the audio element.
  </audio>

  <script>
    const video = document.getElementById("myVideo");
    const audio = document.getElementById("myAudio");

    function playMedia() {
      video.play();
      audio.play().catch((error) => {
        console.log("Audio play blocked by browser: ", error);
      });
    }

    function stopMedia() {
      video.pause();
      video.currentTime = 0;

      audio.pause();
      audio.currentTime = 0;
    }
  </script>
</body>
</html>
