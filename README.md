<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Happy Birthday Babycat!</title>
  <style>
    body {
      display: flex;
      height: 100vh;
      background: linear-gradient(120deg, #fae7e1, #d2e6fa, #f1c6e7);
      justify-content: center;
      align-items: center;
      font-family: 'Segoe UI', Arial, sans-serif;
      overflow: hidden;
    }
    .envelope {
      width: 320px;
      height: 215px;
      background: #fff;
      border-radius: 12px;
      position: relative;
      box-shadow: 0 16px 32px rgba(0,0,0,.12), 0 4px 8px rgba(0,0,0,.08);
      cursor: pointer;
      transition: 0.3s;
      z-index: 2;
    }
    .flap {
      position: absolute;
      left: 0;
      top: -80px;
      width: 320px;
      height: 120px;
      background: #f5d6ec;
      border-radius: 0 0 40% 40%/0 0 80px 80px;
      transform-origin: bottom;
      transition: 0.7s;
      z-index: 3;
    }
    .envelope.open .flap {
      transform: rotateX(-110deg);
    }
    .letter {
      width: 90%;
      height: 160px;
      position: absolute;
      left: 5%;
      top: 30px;
      background: #fffdf5;
      box-shadow: 0 2px 8px #fae1f9a9;
      border-radius: 6px;
      padding: 22px 16px;
      box-sizing: border-box;
      opacity: 0;
      transform: translateY(26px);
      transition: 0.8s;
      font-size: 15px;
      color: #614053;
      line-height: 1.5;
      z-index: 1;
    }
    .envelope.open .letter {
      opacity: 1;
      transform: translateY(-14px);
      transition-delay: 0.5s;
    }
    .heart {
        position: absolute;
        top: 20%;
        left: 50%;
        width: 40px;
        height: 40px;
        margin-left: -20px;
        background: none;
        z-index: 10;
        transform: scale(0.9) rotate(-10deg);
        animation: pop 1.6s ease-in-out 1;
    }
    @keyframes pop {
        0% { transform: scale(1.3) rotate(-12deg);}
        60% { transform: scale(0.92) rotate(-15deg);}
        80% { transform: scale(1.08) rotate(-8deg);}
        100% { transform: scale(1) rotate(-10deg);}
    }
    .heart-shape {
      position: absolute;
      width: 40px; height: 40px;
      left: 0; top: 0;
    }
    .heart-shape:before,
    .heart-shape:after {
      content: "";
      position: absolute;
      left: 16px;
      top: 2px;
      width: 18px;
      height: 28px;
      background: #ff719a;
      border-radius: 18px 18px 0 0;
      transform: rotate(-45deg);
    }
    .heart-shape:after {
      left: 4px;
      transform: rotate(45deg);
    }
    .open-btn, .close-btn {
      position: absolute;
      bottom: 14px;
      right: 20px;
      padding: 7px 18px;
      background: #f691b4;
      border: none;
      border-radius: 16px;
      color: #fff;
      cursor: pointer;
      font-size: 15px;
      transition: 0.2s;
      opacity: 0.98;
      z-index: 5;
    }
    .close-btn {
      left: 20px;
      right: auto;
      background: #b191f6;
      display: none;
    }
    .envelope.open .open-btn { display: none; }
    .envelope.open .close-btn { display: block; }
    @media (max-width: 480px) {
      .envelope { width: 94vw; height: 120vw; max-width: 96vw; max-height: 340vw; }
      .flap, .letter { width: 100%; left: 0; }
    }
  </style>
</head>
<body>
  <div class="envelope" id="envelope">
    <div class="flap"></div>
    <div class="heart">
      <div class="heart-shape"></div>
    </div>
    <div class="letter">
      <b>dear my babycat,</b><br>
      happy birthday to my most loveliest silly baby ever, i'm so happy i can spend your 21st birthday with me right now, i'm really happy you still stay becoming my wife until now.<br>
      i'm so sorry me still bad wifey, but me tryieeee, me will try so hard to become the best voidie cattt for you, please wait until im settled in to move in with you, i will make you the best woman ever.<br>
      and remember i dont want anyone else but with your silly ass catt, hehehehe, i hope you will get what u want very easily, and achieve your dreamssss with meee, xoxo voidie cat
    </div>
    <button class="open-btn" onclick="openLetter()">Open Letter</button>
    <button class="close-btn" onclick="closeLetter()">Close</button>
  </div>

  <script>
    function openLetter() {
      document.getElementById('envelope').classList.add('open');
    }
    function closeLetter() {
      document.getElementById('envelope').classList.remove('open');
    }
  </script>
</body>
</html>
