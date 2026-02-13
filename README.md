<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Ask Kiera to Be My Valentine 💘</title>
  <style>
    body {
      text-align: center;
      font-family: Arial, sans-serif;
      background: linear-gradient(135deg, #f8c8d0, #d9b8a8); /* Pink and brown mix */
      color: #333;
      padding-top: 100px;
      position: relative;
      overflow: hidden;
    }
    h1 {
      font-size: 50px;
      color: #b33c5a;
      margin-bottom: 20px;
    }
    p {
      font-size: 24px;
      color: #5c3c3c;
      margin-bottom: 40px;
    }
    button {
      font-size: 22px;
      padding: 15px 30px;
      margin: 20px;
      background-color: #b33c5a;
      color: white;
      border: none;
      border-radius: 10px;
      cursor: pointer;
      transition: background-color 0.3s;
    }
    button:hover {
      background-color: #9a3147;
    }
    #no {
      position: absolute;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -50%);
    }
    audio {
      display: none;
    }
  </style>
</head>
<body>
  <h1>Kiera, Will You Be My Valentine?</h1>
  <p>This moment means so much to me, and I couldn't imagine a better person to share it with.</p>
  <button onclick="yes()">Yes, I Will!</button>
  <button id="no" onmouseover="moveNo()">No, Thanks</button>
  
  <!-- Hidden Audio -->
  <audio id="music" autoplay loop>
    <source src="https://www.bensound.com/bensound-music/bensound-ukulele.mp3" type="audio/mpeg">
    Your browser does not support the audio element.
  </audio>
  
  <!-- Canvas for Confetti -->
  <script src="https://cdn.jsdelivr.net/npm/canvas-confetti@1.5.1/dist/confetti.browser.min.js"></script>
  <script>
    // Function for the "Yes" button
    function yes() {
      confetti({
        particleCount: 200,
        spread: 160,
        origin: { y: 0.6 }
      });
      alert("Best decision ever! 💖 Can't wait for Valentine's Day!");
    }
    
    // Move the "No" button away
    function moveNo() {
      const noButton = document.getElementById('no');
      noButton.style.top = Math.random() * 80 + '%';
      noButton.style.left = Math.random() * 80 + '%';
    }
  </script>
</body>
</html>
