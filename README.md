<!DOCTYPE html>
<html lang="kn">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Birthday Tease 😏</title>
  <style>
    body {
      margin: 0;
      min-height: 100vh;
      display: flex;
      justify-content: center;
      align-items: center;
      background: linear-gradient(135deg, #fde68a, #fca5a5);
      font-family: 'Poppins', sans-serif;
    }
    .card {
      background: white;
      width: 90%;
      max-width: 420px;
      padding: 25px;
      border-radius: 20px;
      text-align: center;
      box-shadow: 0 20px 40px rgba(0,0,0,0.2);
    }
    button {
      padding: 12px 18px;
      border: none;
      border-radius: 12px;
      font-size: 1rem;
      cursor: pointer;
      margin: 8px;
      background: #fb7185;
      color: white;
    }
    .hidden { display: none; }
    img {
      width: 100%;
      border-radius: 16px;
      margin-top: 15px;
    }
    .final {
      font-size: 1.8rem;
      color: #ef4444;
    }
  </style>
</head>
<body>

  <!-- Screen 1 -->
  <div class="card" id="s1">
    <h2>😎 ಒಂದು ಸಣ್ಣ ಪ್ರಶ್ನೆ</h2>
    <p><strong>ನೀನು ಎಷ್ಟು cool ಅಂತ ಭಾವಿಸ್ತೀಯಾ?</strong></p>
    <button onclick="wrong('ಸುಳ್ಳು ಹೇಳ್ಬೇಡ 😌')">ತುಂಬಾ cool 😎</button>
    <button onclick="wrong('ಅಯ್ಯೋ! ನಿಜಾನಾ? 🤨')">ಸ್ವಲ್ಪ cool 😏</button>
    <button onclick="next()">ಹಾಗೇನೋ 😌</button>
  </div>

  <!-- Screen 2 -->
  <div class="card hidden" id="s2">
    <h2>🤔 ಗಂಭೀರ ಪ್ರಶ್ನೆ</h2>
    <p><strong>ನಿನ್ನನ್ನು ಹೆಚ್ಚು ಕಿರಿಕಿರಿ ಮಾಡೋದು ಯಾರು?</strong></p>
    <button onclick="wrong('ಸುಳ್ಳು ಪತ್ತೆ ಆಯ್ತು 🚨')">ನನ್ನ ಸ್ನೇಹಿತರು</button>
    <button onclick="wrong('ಇದು ನಂಬಲು ಆಗಲ್ಲ 😒')">ನನ್ನ ಫ್ಯಾಮಿಲಿ</button>
    <button onclick="next2()">ನೀನೇ 🙃</button>
  </div>

  <!-- Screen 3 -->
  <div class="card hidden" id="s3">
    <h2>😈 ಕೊನೆ ಪ್ರಶ್ನೆ</h2>
    <p><strong>ಇವತ್ತು ನೀನು cake ಗೆ ಅರ್ಹನೇ?</strong></p>
    <button onclick="next3()">ಹೌದು obviously 🍰</button>
    <button onclick="wrong('ಅದ್ರೇ ಹಾಗಿದ್ರೆ cake ಇಲ್ಲ 😌')">ಇಲ್ಲ 😔</button>
  </div>

  <!-- Final -->
  <div class="card hidden" id="final">
    <h1 class="final">🎉 Happy Birthday! 🎉</h1>
    <p>ಸರಿ ಸರಿ… ಜೋಕ್ ಸಾಕು 😄</p>
    <p>ನಿನ್ನ ಜೀವನದಲ್ಲಿ ಸದಾ ನಗು, ಸಂತೋಷ ಮತ್ತು success ಇರಲಿ ✨</p>
    <p>ಹೀಗೇ ಇದ್ದೇ ಇರು (ಸ್ವಲ್ಪ annoying ಆದ್ರೂ 😏)</p>

    <!-- Insert his photo here -->
    <img src="him.jpg" alt="Birthday Photo" />

    <p style="margin-top:10px;">– ನನ್ನ ಕಿರಿಕಿರಿಯನ್ನು ಸಹಿಸುವ ಒಬ್ಬ 😏</p>
  </div>

  <script>
    function wrong(msg) { alert(msg); }
    function next() { s1.classList.add('hidden'); s2.classList.remove('hidden'); }
    function next2() { s2.classList.add('hidden'); s3.classList.remove('hidden'); }
    function next3() { s3.classList.add('hidden'); final.classList.remove('hidden'); }
  </script>

</body>
</html>
