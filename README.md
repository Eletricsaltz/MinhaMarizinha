<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>EU TE AMO, MARIANA!</title>
    <style>
        body {
            background-color: #ffe6e6;
            font-family: 'Cursive', sans-serif;
            color: #ff3366;
            text-align: center;
            overflow: hidden;
        }
        h1 {
            font-size: 3rem;
            margin-top: 20px;
            color: #ff3366;
            animation: pulse 2s infinite;
        }
        .love-message {
            font-size: 1.7rem;
            margin: 10px 0;
        }
        .heart {
            color: #ff3366;
            font-size: 2rem;
            animation: pulse 1.5s infinite;
        }
        @keyframes pulse {
            0% {
                transform: scale(1);
            }
            50% {
                transform: scale(1.1);
            }
            100% {
                transform: scale(1);
            }
        }
        /* Coracoes flutuantes */
        .floating-heart {
            position: fixed;
            color: red;
            font-size: 1.5rem;
            animation: float 5s infinite ease-in-out;
            bottom: -50px;
        }
        @keyframes float {
            0% {
                opacity: 0;
                transform: translateX(0) translateY(0);
            }
            50% {
                opacity: 1;
            }
            100% {
                opacity: 0;
                transform: translateX(50px) translateY(-700px);
            }
        }
        /* Várias animações de corações */
        .heart1 {
            left: 20%;
            animation-duration: 5s;
        }
        .heart2 {
            left: 50%;
            animation-duration: 6s;
        }
        .heart3 {
            left: 80%;
            animation-duration: 7s;
        }
        .heart4 {
            left: 35%;
            animation-duration: 8s;
        }
        .heart5 {
            left: 65%;
            animation-duration: 9s;
        }
    </style>
</head>
<body>
    <h1>❤️ EU TE AMO, MARIANA! ❤️</h1>
    <div id="messages"></div>

    <script>
        const messagesDiv = document.getElementById("messages");
        for (let i = 0; i < 500; i++) {
            const message = document.createElement("p");
            message.classList.add("love-message");
            message.innerHTML = "EU TE AMO, MARIANA! ❤️";
            messagesDiv.appendChild(message);
        }

        // Função para criar corações flutuantes
        function createHeart(className) {
            const heart = document.createElement("div");
            heart.classList.add("floating-heart", className);
            heart.innerHTML = "❤️";
            document.body.appendChild(heart);
        }

        // Criando vários corações flutuantes
        createHeart('heart1');
        createHeart('heart2');
        createHeart('heart3');
        createHeart('heart4');
        createHeart('heart5');
    </script>
</body>
</html>
