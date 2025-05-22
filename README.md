<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Audio Play Button</title>
</head>
<body>
  <h1>Welcome to My GitHub Page</h1>
  <button onclick="playAudio()">Play Audio</button>

  <audio id="myAudio">
    <source src="Crystal Castles KEROSENE Official.mp3" type="audio/mpeg">
    Your browser does not support the audio element.
  </audio>

  <script>
    function playAudio() {
      document.getElementById("myAudio").play();
    }
  </script>
</body>
</html>
