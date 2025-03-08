<!DOCTYPE html>
<html lang="kk">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>8 Наурызға шақыру</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            background: linear-gradient(135deg, #ff0000, #ee0979);
            color: white;
            padding: 35px;
            overflow: hidden;
        }
        .container {
            max-width: 500px;
            margin: auto;
            background: rgba(255, 255, 255, 0.2);
            padding: 35px;
            border-radius: 15px;
            box-shadow: 0px 0px 15px rgba(255, 255, 255, 0.3);
            position: center;
            z-index: 2;
        }
        h1 {
            font-size: 35px;
        }
        p {
            font-size: 20px;
        }
        .date-time {
            font-size: 22px;
            font-weight: bold;
            margin: 15px 0;
        }
        .hearts {
            font-size: 30px;
            margin: 10px 0;
        }
        .address a {
            color: #ffdd57;
            text-decoration: none;
            font-weight: bold;
        }
        .heart {
            position: absolute;
            color: rgb(255, 0, 221);
            font-size: 35px;
            animation: float 5s linear infinite;
        }
        @keyframes float {
            0% { transform: translateY(0) scale(1); opacity: 1; }
            100% { transform: translateY(-100vh) scale(1.5); opacity: 0; }
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Құрметті ханымдар! 💐</h1>
        <p>Сіздерді 8 Наурыз Халықаралық әйелдер күніне арналған мерекелік кешке шақырамыз!</p>
        <div class="date-time">9 наурыз 2025 жыл, 17:54</div>
        <p>Өтетін орын: Караоке Grand Limo</p>
        <p class="address">Толық мекенжай: <a href="https://2gis.kz/almaty/geo/70000001029182219" target="_blank">Картада қарау</a></p>
        <p>Сіздерді керемет тосын сыйлар, жандандыратын музыка және көтеріңкі көңіл-күй күтеді!</p>
        <div class="hearts">❤️❤️❤️</div>
    </div>
    <script>
        function createHeart() {
            const heart = document.createElement("div");
            heart.classList.add("heart");
            heart.innerHTML = "❤️";
            heart.style.left = Math.random() * 100 + "vw";
            heart.style.animationDuration = Math.random() * 3 + 2 + "s";
            document.body.appendChild(heart);
            setTimeout(() => { heart.remove(); }, 5000);
        }
        setInterval(createHeart, 300);
    </script>
</body>
</html>
