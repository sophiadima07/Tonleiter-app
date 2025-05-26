<!DOCTYPE html>
<html lang="de">
<head>
    <meta charset="UTF-8">
    <title>🎼 Tonleiter-Entdecker</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f0f8ff;
            text-align: center;
            padding: 20px;
        }
        h1 {
            color: #2a5d84;
        }
        .note-buttons {
            margin-top: 30px;
        }
        button {
            margin: 10px;
            padding: 20px;
            font-size: 18px;
            border-radius: 10px;
            border: none;
            background-color: #ffde59;
            box-shadow: 2px 2px 5px #999;
            cursor: pointer;
        }
        button:hover {
            background-color: #ffd700;
        }
        audio {
            display: none;
        }
    </style>
</head>
<body>
    <h1>🎼 Entdecke die C-Dur-Tonleiter</h1>
    <p>Klicke auf die Töne und höre dir an, wie die Tonleiter klingt!</p>
    <div class="note-buttons">
        <button onclick="playSound('c')">C</button>
        <button onclick="playSound('d')">D</button>
        <button onclick="playSound('e')">E</button>
        <button onclick="playSound('f')">F</button>
        <button onclick="playSound('g')">G</button>
        <button onclick="playSound('a')">A</button>
        <button onclick="playSound('h')">H</button>
        <button onclick="playSound('c1')">C'</button>
    </div>

    <!-- Audiodateien -->
    <audio id="c" src="sounds/c.mp3"></audio>
    <audio id="d" src="sounds/d.mp3"></audio>
    <audio id="e" src="sounds/e.mp3"></audio>
    <audio id="f" src="sounds/f.mp3"></audio>
    <audio id="g" src="sounds/g.mp3"></audio>
    <audio id="a" src="sounds/a.mp3"></audio>
    <audio id="h" src="sounds/h.mp3"></audio>
    <audio id="c1" src="sounds/c1.mp3"></audio>

    <script>
        function playSound(note) {
            const audio = document.getElementById(note);
            audio.currentTime = 0;
            audio.play();
        }
    </script>
</body>
</html>
