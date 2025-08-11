<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Selamat Ulang Tahun Keyla 🎉</title>
    <style>
        body {
            margin: 0;
            height: 100vh;
            background: linear-gradient(45deg, #ffafbd, #ffc3a0);
            overflow: hidden;
            display: flex;
            justify-content: center;
            align-items: center;
            font-family: Arial, sans-serif;
        }
        h1 {
            font-size: 2.5rem;
            color: white;
            text-shadow: 0 0 10px #ff5e78, 0 0 20px #ff5e78, 0 0 30px #ff5e78;
            animation: glow 1.5s infinite alternate;
            text-align: center;
        }
        @keyframes glow {
            from { text-shadow: 0 0 10px #ff5e78; }
            to { text-shadow: 0 0 20px #ff1e40, 0 0 30px #ff1e40; }
        }
        .heart {
            position: absolute;
            color: #ff5e78;
            font-size: 20px;
            animation: fall 5s linear infinite;
        }
        @keyframes fall {
            0% { transform: translateY(-100px) rotate(0deg); opacity: 1; }
            100% { transform: translateY(100vh) rotate(360deg); opacity: 0; }
        }
    </style>
</head>
<body>
    <h1>🎂 Selamat Ulang Tahun, Keyla! 🎂<br>Semoga selalu bahagia 💖</h1>
    <audio autoplay loop>
        <source src="https://www.bensound.com/bensound-music/bensound-sunny.mp3" type="audio/mpeg">
    </audio>
    <script>
        function createHeart() {
            const heart = document.createElement("div");
            heart.classList.add("heart");
            heart.innerHTML = "💖";
            heart.style.left = Math.random() * 100 + "vw";
            heart.style.fontSize = Math.random() * 20 + 10 + "px";
            document.body.appendChild(heart);
            setTimeout(() => heart.remove(), 5000);
        }
        setInterval(createHeart, 300);
    </script>
</body>
</html>
