<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Happy 30th Birthday, Heckel!</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.2/css/all.min.css">
    <style>
        body {
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            background-color: #1e1e2e;
            flex-direction: column;
            overflow: hidden;
            color: #ffffff;
            font-family: 'Arial', sans-serif;
        }
        h1 {
            font-size: 2.5em;
            color: #ffcc00;
            text-align: center;
        }
        .love {
            position: absolute;
            font-size: 2rem;
            color: red;
            animation: floatUp 3s linear infinite;
        }
        @keyframes floatUp {
            0% { transform: translateY(0); opacity: 1; }
            100% { transform: translateY(-100vh); opacity: 0; }
        }
        button {
            margin-top: 20px;
            padding: 10px 20px;
            font-size: 1.2em;
            background-color: #ffcc00;
            color: black;
            border: none;
            cursor: pointer;
            border-radius: 10px;
        }
        #message {
            max-width: 600px;
            text-align: center;
            margin-top: 20px;
            font-size: 1.1em;
        }
        .game-container {
            margin-top: 30px;
            text-align: center;
        }
        .heart {
            width: 50px;
            height: 50px;
            background-color: red;
            position: absolute;
            border-radius: 50%;
            cursor: pointer;
        }
    </style>
</head>
<body>
    <h1>Happy 30th Birthday, Heckel! 🎉</h1>
    <p id="message">
        HAPPY BIRTHDAY HABIBIE ✨✨✨🥳🥳<br><br>
        Di antara jutaan kemungkinan, semesta menuntun aku ke kamu dan setiap hari sejak itu, aku selalu sadar betapa beruntungnya aku memiliki kamu bukan hanya sebagai pasangan, tapi sebagai tempat aku kembali, sebagai seseorang yang memahami aku bahkan tanpa aku harus bicara.<br><br>
        Aku tahu perjalanan kita tidak selalu mudah. Kita melewati begitu banyak hal, baik yang indah maupun yang sulit. Ada hari-hari di mana segalanya terasa ringan, tapi ada juga hari-hari di mana semuanya terasa melelahkan. Namun, satu hal yang selalu membuat aku yakin adalah kamu tetap bertahan, tetap percaya, tetap menggenggam aku dengan segala lebih dan kurangku. Aku tahu itu tidak selalu mudah, dan aku berhutang terima kasih untuk setiap saat kamu memilih tetap ada.<br><br>
        Makasih untuk kesabaranmu, untuk setiap pelukan yang membuat dunia terasa lebih damai, untuk setiap kata yang menenangkan, untuk cinta yang kamu beri tanpa syarat. Aku tidak pernah meminta apa pun dari semesta selain satu hal: semoga aku bisa selalu membuatmu bahagia, semoga aku bisa selalu menjadi tempat yang nyaman untukmu, seperti kamu untukku.<br><br>
        Di usia yang baru ini, aku hanya ingin kamu tahu betapa kamu berarti. Kamu adalah hal terbaik yang pernah terjadi dalam hidup aku. Dan tidak peduli seberapa banyak waktu berlalu, aku akan selalu ada, selalu menggenggam tanganmu, selalu memilih kamu.<br><br>
        Selamat ulang tahun Sayang. Aku mencintaimu, lebih dari yang bisa aku ucapkan 🥺🥺🥺❤❤❤❤❤❤✨✨✨✨✨✨
    </p>
    <button onclick="startGame()">Mainkan Mini Game 🎮</button>
    
    <div class="game-container" id="game"></div>
    
    <audio id="bgMusic" loop>
        <source src="birds_of_a_feather.mp3" type="audio/mpeg">
    </audio>
    
    <script>
        function createHeart() {
            const heart = document.createElement("div");
            heart.classList.add("love");
            heart.innerHTML = "❤️";
            heart.style.left = Math.random() * 100 + "vw";
            heart.style.top = "100vh";
            document.body.appendChild(heart);
            setTimeout(() => heart.remove(), 3000);
        }
        setInterval(createHeart, 500);

        function startGame() {
            const gameContainer = document.getElementById("game");
            gameContainer.innerHTML = "<p>Temukan hati tersembunyi! Klik hati sebanyak mungkin dalam 10 detik! ❤️</p>";
            let score = 0;
            let startTime = Date.now();

            function createGameHeart() {
                const heart = document.createElement("div");
                heart.classList.add("heart");
                heart.style.left = Math.random() * 80 + "vw";
                heart.style.top = Math.random() * 80 + "vh";
                document.body.appendChild(heart);

                heart.addEventListener("click", () => {
                    score++;
                    heart.remove();
                });
                
                setTimeout(() => heart.remove(), 3000);
            }

            const interval = setInterval(createGameHeart, 500);
            setTimeout(() => {
                clearInterval(interval);
                alert("Game selesai! Kamu berhasil mengumpulkan " + score + " hati! ❤️");
            }, 10000);
        }
    </script>
</body>
</html>
