<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>¡Feliz Cumpleaños!</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            background-color: #ffe4e1;
            overflow: hidden;
            margin: 0;
        }
        h1 {
            color: #ff1493;
            font-size: 3em;
            margin-top: 50px;
            animation: bounce 2s infinite;
        }
        p {
            font-size: 1.2em;
            color: #555;
        }
        button {
            background-color: #ff69b4;
            color: white;
            border: none;
            padding: 10px 20px;
            font-size: 1em;
            border-radius: 20px;
            cursor: pointer;
            box-shadow: 0 4px #ff1493;
            transition: transform 0.2s, box-shadow 0.2s;
        }
        button:hover {
            transform: scale(1.1);
        }
        button:active {
            transform: scale(1);
            box-shadow: 0 2px #ff1493;
        }
        #heart-container {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            pointer-events: none;
        }
        .heart {
            position: absolute;
            width: 20px;
            height: 20px;
            background-color: #ff1493;
            transform: rotate(45deg);
            animation: float 2.5s ease-in-out infinite;
        }
        .heart::before, .heart::after {
            content: "";
            position: absolute;
            width: 20px;
            height: 20px;
            background-color: #ff1493;
            border-radius: 50%;
        }
        .heart::before {
            top: -10px;
            left: 0;
        }
        .heart::after {
            top: 0;
            left: -10px;
        }
        @keyframes bounce {
            0%, 100% {
                transform: translateY(0);
            }
            50% {
                transform: translateY(-20px);
            }
        }
        @keyframes float {
            0% {
                opacity: 1;
                transform: translateY(0) scale(1);
            }
            100% {
                opacity: 0;
                transform: translateY(-200px) scale(0.5);
            }
        }
        #message {
            display: none;
            margin-top: 30px;
            font-size: 1.2em;
            color: #ff1493;
        }
    </style>
</head>
<body>
    <h1>🎉 ¡Feliz Cumpleaños, Amiga! 🎉</h1>
    <p>Espero que tengas un día increíble lleno de sorpresas.</p>
    <button onclick="showLove()">Presiona aquí para descubrir algo especial</button>
    
    <div id="heart-container"></div>
    <p id="message">
        Querida amiga, <br>
        En este día tan especial, quiero recordarte lo importante que eres para mí. Eres una persona increíble, llena de luz, risas y amor. Espero que este día esté lleno de sorpresas, alegría y todos esos pequeños momentos que hacen que la vida sea maravillosa. Gracias por ser tú, por estar siempre y por hacer de cada día algo mejor. ¡Te quiero mucho! ❤️
    </p>

    <script>
        let intervalId;

        function createHeart() {
            const heartContainer = document.getElementById('heart-container');
            const heart = document.createElement('div');
            heart.className = 'heart';
            heart.style.left = Math.random() * 100 + 'vw';
            heart.style.animationDuration = Math.random() * 2 + 2 + 's';
            heartContainer.appendChild(heart);
            setTimeout(() => {
                heart.remove();
            }, 2500);
        }

        function showLove() {
            const message = document.getElementById('message');
            if (message.style.display === 'none') {
                message.style.display = 'block';
                intervalId = setInterval(createHeart, 200);
            }
        }
    </script>
</body>
</html>
