<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Text Animation</title>
    <style>
        body {
            margin: 0;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            background: linear-gradient(135deg, #1e3c72, #2a5298);
            overflow: hidden;
            font-family: 'Arial', sans-serif;
        }

        .text-container {
            position: relative;
            font-size: 3rem;
            font-weight: bold;
            color: white;
            text-transform: uppercase;
            letter-spacing: 5px;
        }

        .text-container span {
            display: inline-block;
            opacity: 0;
            transform: translateY(30px);
            animation: fadeInUp 1s ease forwards;
        }

        .text-container span:nth-child(1) {
            animation-delay: 0.2s;
        }
        .text-container span:nth-child(2) {
            animation-delay: 0.4s;
        }
        .text-container span:nth-child(3) {
            animation-delay: 0.6s;
        }
        .text-container span:nth-child(4) {
            animation-delay: 0.8s;
        }
        .text-container span:nth-child(5) {
            animation-delay: 1s;
        }
        .text-container span:nth-child(6) {
            animation-delay: 1.2s;
        }
        .text-container span:nth-child(7) {
            animation-delay: 1.4s;
        }

        @keyframes fadeInUp {
            0% {
                opacity: 0;
                transform: translateY(30px);
            }
            100% {
                opacity: 1;
                transform: translateY(0);
            }
        }

        .glow {
            text-shadow: 0 0 10px #ffffff, 0 0 20px #ff0099, 0 0 30px #ff0099, 0 0 40px #ff0099;
            animation: glowEffect 1.5s infinite alternate;
        }

        @keyframes glowEffect {
            0% {
                text-shadow: 0 0 10px #ffffff, 0 0 20px #ff0099, 0 0 30px #ff0099, 0 0 40px #ff0099;
            }
            100% {
                text-shadow: 0 0 20px #ffffff, 0 0 30px #ff33cc, 0 0 40px #ff33cc, 0 0 50px #ff33cc;
            }
        }
    </style>
</head>
<body>
    <div class="text-container">
        <span class="glow">H</span>
        <span class="glow">i</span>
        <span>,</span>
        <span class="glow">I</span>
        <span class="glow">'m</span>
        <span class="glow">S</span>
        <span class="glow">u</span>
        <span class="glow">s</span>
        <span class="glow">h</span>
        <span class="glow">a</span>
        <span class="glow">n</span>
    </div>
</body>
</html>
