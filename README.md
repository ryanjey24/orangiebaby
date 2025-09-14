<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Happy Birthday BabyCat! 🎂</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            font-family: 'Arial Rounded MT Bold', 'Arial', sans-serif;
            background: linear-gradient(135deg, #1a1a2e 0%, #16213e 100%);
            color: #fff;
            min-height: 100vh;
            overflow-x: hidden;
            display: flex;
            justify-content: center;
            align-items: center;
            padding: 20px;
        }
        
        .container {
            max-width: 800px;
            width: 100%;
            background: rgba(30, 30, 50, 0.8);
            border-radius: 20px;
            padding: 30px;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.5);
            position: relative;
            overflow: hidden;
            border: 3px solid #ff9ecb;
        }
        
        .envelope {
            position: relative;
            cursor: pointer;
            text-align: center;
            margin-bottom: 30px;
            transition: transform 0.3s;
        }
        
        .envelope:hover {
            transform: scale(1.05);
        }
        
        .envelope-img {
            width: 200px;
            filter: drop-shadow(0 5px 15px rgba(255, 158, 203, 0.5));
        }
        
        .letter {
            display: none;
            background: rgba(255, 240, 245, 0.95);
            color: #333;
            padding: 30px;
            border-radius: 15px;
            margin-top: 20px;
            box-shadow: 0 5px 20px rgba(0, 0, 0, 0.2);
            border: 2px solid #ff9ecb;
            position: relative;
        }
        
        .letter-text {
            line-height: 1.8;
            font-size: 18px;
            text-align: center;
        }
        
        .signature {
            text-align: right;
            font-style: italic;
            margin-top: 20px;
            font-weight: bold;
            color: #ff6b9d;
        }
        
        h1 {
            text-align: center;
            color: #ff6b9d;
            margin-bottom: 30px;
            font-size: 36px;
            text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.3);
        }
        
        .hearts {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            pointer-events: none;
            z-index: -1;
        }
        
        .heart {
            position: absolute;
            width: 20px;
            height: 20px;
            background: #ff6b9d;
            transform: rotate(45deg);
            opacity: 0;
            animation: fall 5s linear infinite;
        }
        
        .heart:before, .heart:after {
            content: '';
            width: 20px;
            height: 20px;
            background: #ff6b9d;
            border-radius: 50%;
            position: absolute;
        }
        
        .heart:before {
            top: -10px;
            left: 0;
        }
        
        .heart:after {
            top: 0;
            left: -10px;
        }
        
        @keyframes fall {
            0% {
                top: -10%;
                opacity: 1;
            }
            100% {
                top: 100%;
                opacity: 0;
            }
        }
        
        .kiss {
            position: absolute;
            font-size: 24px;
            opacity: 0;
            color: #ff6b9d;
        }
        
        .cat {
            position: absolute;
            font-size: 30px;
            bottom: 20px;
            right: 20px;
            animation: bounce 2s infinite;
        }
        
        @keyframes bounce {
            0%, 100% {
                transform: translateY(0);
            }
            50% {
                transform: translateY(-10px);
            }
        }
        
        .instructions {
            text-align: center;
            margin-top: 20px;
            color: #ff9ecb;
            font-size: 16px;
        }
        
        @media (max-width: 600px) {
            h1 {
                font-size: 28px;
            }
            
            .letter-text {
                font-size: 16px;
            }
            
            .container {
                padding: 20px;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Happy 21st Birthday BabyCat! 🎂</h1>
        
        <div class="envelope" onclick="openLetter()">
            <img src="data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCA1MTIgNTEyIj48cGF0aCBmaWxsPSIjZmY5ZWNiIiBkPSJNNDU2LDgwSDYwQzQ4LjkyOCw4MCw0MCw4OC45MjgsNDAsMTAwdjI3MmMwLDExLjA3Miw4LjkyOCwyMCwyMCwyMGgzOTZjMTEuMDcyLDAsMjAtOC45MjgsMjAtMjBWMTIwQzQ4MCw4OC45MjgsNDcxLjA3Miw4MCw0NTYsODB6IE00NTYsMTQwTDI3OC4zNjgsMjk1LjQ4Yy00LjY0NCwzLjUzNi0xMS4zMTIsMy41MzYtMTUuOTU2LDBINTZWMTE2aDQwMFYxNDB6IiAvPjwvc3ZnPg==" alt="Envelope" class="envelope-img">
            <p class="instructions">Click the envelope to open your letter!</p>
        </div>
        
        <div class="letter" id="letter">
            <div class="letter-text">
                <p>Dear my BabyCat,</p>
                <p>Happy birthday to my most loveliest silly baby ever!</p>
                <p>I'm so happy I can spend your 21st birthday with me right now,</p>
                <p>I'm really happy you still stay becoming my wife until now,</p>
                <p>I'm so sorry me still bad wifey, but me tryieeee,</p>
                <p>Me will try so hard to become the best voidie cattt for you,</p>
                <p>Please wait until I'm settled in to move in with you,</p>
                <p>I will make you the best woman ever,</p>
                <p>And remember I don't want anyone else but with your silly ass catt, hehehehe,</p>
                <p>I hope you will get what u want very easily,</p>
                <p>And achieve your dreamssss with meee,</p>
                <p class="signature">xoxo voidie cat</p>
            </div>
        </div>
        
        <div class="cat">😻</div>
    </div>
    
    <div class="hearts" id="hearts"></div>
    
    <script>
        function openLetter() {
            const letter = document.getElementById('letter');
            const envelope = document.querySelector('.envelope');
            
            if (letter.style.display === 'block') {
                return;
            }
            
            letter.style.display = 'block';
            envelope.style.display = 'none';
            
            createHearts();
            createKisses();
            
            // Play meow sound
            const audio = new Audio('data:audio/mp3;base64,SUQzBAAAAAAAI1RTU0UAAAAPAAADTGF2ZjU4Ljc2LjEwMAAAAAAAAAAAAAAA/+M4wAAAAAAAAAAAAEluZm8AAAAPAAAAAwAAAbkAVVVVVVVVVVVVVVVVVVVVVVVVVVVVVVVVVVVVVVVVVVVVVVVVVVVVVVVVVVVVVVVV///////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////8AAAAATGF2YzU4LjEzAAAAAAAAAAAAAAAAJAUHg//M4wDsAAAaPAUAAAAMExBTQIggKEggBNAYEBgECBgQCBgQGAQIGAgIGAQIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAgIGAg
