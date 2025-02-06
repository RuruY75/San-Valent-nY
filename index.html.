<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>San Valentín ❤️</title>
    <style>
        body {
            font-family: 'Comic Sans MS', cursive, sans-serif;
            text-align: center;
            background: linear-gradient(135deg, #ffb6c1, #ff69b4);
            color: white;
            overflow: hidden;
        }
        .container {
            margin-top: 50px;
            padding: 20px;
        }
        h1 {
            font-size: 2.5em;
            text-shadow: 2px 2px 4px rgba(0,0,0,0.3);
        }
        .heart {
            font-size: 50px;
            animation: heartbeat 1s infinite alternate;
        }
        @keyframes heartbeat {
            from { transform: scale(1); }
            to { transform: scale(1.2); }
        }
        .buttons {
            margin-top: 20px;
        }
        button {
            font-size: 18px;
            padding: 10px 20px;
            margin: 10px;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            transition: 0.3s;
        }
        .yes {
            background-color: #ff4d79;
            color: white;
        }
        .yes:hover {
            background-color: #ff1e56;
        }
        .no {
            background-color: #ccc;
            color: black;
            position: absolute;
        }
        #snoopy {
            width: 150px;
            margin-top: 20px;
            animation: float 3s ease-in-out infinite;
        }
        @keyframes float {
            0%, 100% { transform: translateY(0); }
            50% { transform: translateY(-10px); }
        }
        .message {
            font-size: 1.5em;
            margin-top: 20px;
            display: none;
        }
        /* Corazones cayendo */
        .heart-fall {
            position: absolute;
            top: -50px;
            color: red;
            font-size: 20px;
            animation: fall 5s linear infinite;
        }
        @keyframes fall {
            from { transform: translateY(-50px); }
            to { transform: translateY(100vh); }
        }
    </style>
    <script>
        function showYesMessage() {
            document.getElementById("message").innerHTML = "¡Sabía que dirías que sí, Yamanys! ❤️ Te quiero mucho 🥰";
            document.getElementById("message").style.display = "block";
            createHearts();
        }

        function moveNoButton() {
            let button = document.getElementById("noBtn");
            let x = Math.random() * (window.innerWidth - 100);
            let y = Math.random() * (window.innerHeight - 50);
            button.style.left = x + "px";
            button.style.top = y + "px";
        }

        function showNoMessage() {
            document.getElementById("message").innerHTML = "😢 Bueno... aún así, siempre serás especial para mí 💔";
            document.getElementById("message").style.display = "block";
        }

        function createHearts() {
            for (let i = 0; i < 30; i++) {
                let heart = document.createElement("div");
                heart.innerHTML = "❤️";
                heart.classList.add("heart-fall");
                heart.style.left = Math.random() * 100 + "vw";
                heart.style.animationDuration = (Math.random() * 3 + 2) + "s";
                document.body.appendChild(heart);
                setTimeout(() => heart.remove(), 5000);
            }
        }
    </script>
</head>
<body>
    <div class="container">
        <h1>Yamanys, ¿quieres ser mi San Valentín? ❤️</h1>
        <img id="snoopy" src="https://upload.wikimedia.org/wikipedia/commons/5/5f/Snoopy_Peanuts.svg" alt="Snoopy">
        <div class="buttons">
            <button class="yes" onclick="showYesMessage()">Sí</button>
            <button class="no" id="noBtn" onmouseover="moveNoButton()" onclick="showNoMessage()">No</button>
        </div>
        <p id="message" class="message"></p>
    </div>
</body>
</html>
