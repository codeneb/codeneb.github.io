<!DOCTYPE html>
<html>
    <head>
        <meta charset="utf-8">
        <title>koneb's devpage</title>
    </head>
    <body>
        <h1>koneb</h1>
        <h2>welcome to my devpage!</h2>
        <p>business email: konebstreaming@gmail.com</p>
        <h2>about me</h2>
        <p>beginner programmer, currently learning python</p>
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
    </body>
</html>
