<!DOCTYPE html>
<html>
    <head>
        <meta charset="utf-8">
        <title>koneb's devpage</title>
        <link href="https://fonts.googleapis.com/css2?family=Open+Sans:wght@400;600&display=swap" rel="stylesheet">
        <style>
            body {
                font-family: 'Open Sans', sans-serif;
            }
            button {
                background-color: lightgreen;
                color: darkgreen;
                border: none;
                padding: 10px 20px;
                font-size: 16px;
                cursor: pointer;
                border-radius: 5px;
                font-family: 'Open Sans', sans-serif;
                font-weight: 600;
            }
            button:hover {
                background-color: limegreen;
            }
        </style>
    </head>
        <h2>welcome to my devpage!</h2>
        <h2>about me</h2>
        <p>beginner programmer, currently learning python</p>
    <h2>funy button</h2>
        <button onclick="playSound()">yippey</button>
        <audio id="yippey-sound">
            <source src="yippee-made-with-Voicemod.mp3" type="audio/mpeg">
            Your browser does not support the audio element.
        </audio>
        <script>
            function playSound() {
                var sound = document.getElementById("yippey-sound");
                sound.play();
            }
        </script>
    <body>
        <h2>silly cat images</h2>
        <img src="download (27).jpeg" alt="Profile Image" width="300">
        <img src="😴.jpeg" alt="Sleeping Cat" width="300">
    </body>
</html>
