# valintine-2026
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Happy Valentine's Day!</title>
    <style>
        body {
            font-family: 'Arial', sans-serif;
            background: linear-gradient(to bottom, #ffcccc, #ff9999);
            color: #d63384;
            text-align: center;
            margin: 0;
            padding: 20px;
            overflow-x: hidden;
        }
        .login-container {
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            background: rgba(255, 255, 255, 0.8);
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            z-index: 10;
        }
        .login-box {
            background: white;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0 0 10px rgba(0,0,0,0.2);
        }
        input[type="password"] {
            padding: 10px;
            margin: 10px 0;
            border: 1px solid #d63384;
            border-radius: 5px;
        }
        button {
            background: #d63384;
            color: white;
            border: none;
            padding: 10px 20px;
            border-radius: 5px;
            cursor: pointer;
        }
        button:hover {
            background: #b0246a;
        }
        .main-content {
            display: none;
        }
        h1 {
            font-size: 2.5em;
            margin-bottom: 20px;
        }
        .message {
            font-size: 1.2em;
            margin: 20px 0;
            font-style: italic;
        }
        .photos {
            display: flex;
            justify-content: center;
            flex-wrap: wrap;
            gap: 20px;
            margin: 20px 0;
        }
        .photos img {
            width: 200px;
            height: 200px;
            object-fit: cover;
            border-radius: 10px;
            box-shadow: 0 0 10px rgba(0,0,0,0.2);
        }
        .music {
            margin: 20px 0;
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
            color: #ff69b4;
            font-size: 2em;
            animation: float 5s infinite ease-in-out;
        }
        @keyframes float {
            0%, 100% { transform: translateY(0); }
            50% { transform: translateY(-20px); }
        }
    </style>
</head>
<body>
    <div class="login-container" id="login">
        <div class="login-box">
            <h2>Enter the Password to Unlock Your Surprise</h2>
            <input type="password" id="password" placeholder="Password">
            <br>
            <button onclick="checkPassword()">Enter</button>
            <p id="error" style="color: red; display: none;">Wrong password! Try again.</p>
        </div>
    </div>

    <div class="main-content" id="content">
        <div class="hearts">
            <!-- Floating hearts animation -->
            <div class="heart" style="left: 10%; animation-delay: 0s;">❤️</div>
            <div class="heart" style="left: 20%; animation-delay: 1s;">💖</div>
            <div class="heart" style="left: 30%; animation-delay: 2s;">❤️</div>
            <div class="heart" style="left: 40%; animation-delay: 3s;">💖</div>
            <div class="heart" style="left: 50%; animation-delay: 4s;">❤️</div>
            <div class="heart" style="left: 60%; animation-delay: 5s;">💖</div>
            <div class="heart" style="left: 70%; animation-delay: 6s;">❤️</div>
            <div class="heart" style="left: 80%; animation-delay: 7s;">💖</div>
            <div class="heart" style="left: 90%; animation-delay: 8s;">❤️</div>
        </div>

        <h1>Happy Valentine's Day, My soulmate! 💕</h1>

        <div class="message">
            " حياتي وروحي كل عيد وكل سنه واحنا مع بعض وبنحب بحض اكتر من اليوم الي قبليه❤️❤️❤️"
        </div>
        <div class="message">
            بصي بقا ايوه احنا مش عارفين امتي بالظبط شوفنا بعض بس دا احلي يوم مر عليا فياتي عرفت في احلي واجمل انسانه في الدنيا ربنا رزقني بيها وربنا ما يحرمني منها ابدا ❤️❤️❤️❤️
        </div>
        <div class="message">
            انسانه قمر واحلي منها مفيش ما شاء الله نورت عليا حياتي محبتش غيرك ولا هحب  حد غيرك حبيتك بجد وعشقتك وبموت فيكي وبغير وبغير وبغير ليا انا وبس ونفس الكلام انا
        </div>
        <div class="massege">
            بحبك اعمل ايه طيب 😂❤️❤️❤️❤️
        </div>

        <div class="photos">
            <img src="https://images.unsplash.com/photo-1518199266791-5375a83190b7?ixlib=rb-4.0.3&auto=format&fit=crop&w=500&q=80" alt="Romantic photo 1">
            <img src="https://images.unsplash.com/photo-1474552226712-ac0f0961a954?ixlib=rb-4.0.3&auto=format&fit=crop&w=500&q=80" alt="Romantic photo 2">
            <img src="https://images.unsplash.com/photo-1516589178581-6cd7833ae3b2?ixlib=rb-4.0.3&auto=format&fit=crop&w=500&q=80" alt="Romantic photo 3">
        </div>

        <div class="music">
            <h2>Listen Our Song 🎶</h2>
            <audio controls autoplay loop>
                <source src="https://drive.google.com/file/d/1uAC8X4_DxGRSHXCl8zSsExJ_wlql-nNe/view?usp=drive_link" type="audio/mpeg">
                <!-- Replace with your own music URL, e.g., an MP3 file -->
                Your browser does not support the audio element.
            </audio>
        </div>
    </div>

    <script>
        function checkPassword() {
            const password = document.getElementById('password').value;
            if (password === '962008') {
                document.getElementById('login').style.display = 'none';
                document.getElementById('content').style.display = 'block';
            } else {
                document.getElementById('error').style.display = 'block';
            }
        }
    </script>
</body>
</html>
