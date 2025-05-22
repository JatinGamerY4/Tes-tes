
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Audio Play/Stop</title>
</head>
<body>
  <h1>Welcome to My GitHub Page</h1>

  <button onclick="playAudio()">Play Audio</button>
  <button onclick="stopAudio()">Stop Audio</button>

  <audio id="myAudio">
    <source src="Crystal Castles KEROSENE Official.mp3" type="audio/mpeg">
    Your browser does not support the audio element.
  </audio>

  <script>
    const audio = document.getElementById("myAudio");

    function playAudio() {
      audio.play();
    }

    function stopAudio() {
      audio.pause();
      audio.currentTime = 0; // Audio ko reset karta hai
    }
  </script>
</body>
</html>
