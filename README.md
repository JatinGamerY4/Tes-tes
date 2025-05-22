<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Play Audio and Video</title>
</head>
<body>
  <h1>Welcome to My GitHub Page</h1>

  <button onclick="playMedia()">Play Audio & Video</button>
  <button onclick="stopMedia()">Stop Audio & Video</button>

  <br><br>

  <video id="myVideo" width="640" controls>
    <source src="Crystal Castles - KEROSENE (Lyrics).mp4" type="video/mp4">
    Your browser does not support the video tag.
  </video>

  <audio id="myAudio">
    <source src="Crystal Castles KEROSENE Official.mp3" type="audio/mpeg">
    Your browser does not support the audio element.
  </audio>

  <script>
    const video = document.getElementById("myVideo");
    const audio = document.getElementById("myAudio");

    function playMedia() {
      audio.play();
      video.play();
    }

    function stopMedia() {
      audio.pause();
      audio.currentTime = 0;

      video.pause();
      video.currentTime = 0;
    }
  </script>
</body>
</html>
