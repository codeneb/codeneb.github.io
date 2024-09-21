<!DOCTYPE html>
<html>
    <head>
        <meta charset="utf-8">
        <title>koneb's devpage</title>
        <link href="https://fonts.googleapis.com/css2?family=Open+Sans:wght@400;600&display=swap" rel="stylesheet">
        <style>
            body {
                font-family: 'Open Sans', sans-serif;
                margin: 20px;
            }
            h1, h2 {
                margin-bottom: 20px; /* Add space below headings */
            }
            p {
                margin-bottom: 20px; /* Add space below paragraphs */
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
                margin-top: 20px; /* Space above the button */
                margin-bottom: 40px; /* Space below the button to separate it from the next section */
            }
            button:hover {
                background-color: limegreen;
            }
            img {
                display: block; /* Display images as block elements */
                margin-bottom: 20px; /* Add space below each image */
            }
        </style>
    </head>
    <body>
        <h1>koneb's devpage</h1>
        <h2>welcome to my devpage!</h2>
        <p>email: konebstreaming@gmail.com</p>
        <h2>about me</h2>
        <p>beginner programmer, currently learning python</p>
        <button onclick="playSound()">yippey</button>
        <audio id="yippey-sound">
            <source src="yippee-made-with-Voicemod.mp3" type="audio/mpeg">
            Your browser does not support the audio element.
        </audio>
}
        <h1>silly cat images</h1>
        <img src="download (27).jpeg" alt="Profile Image" width="300">
        <img src="😴.jpeg" alt="Sleeping Cat" width="300">
   }     
        <script>
            function playSound() {
                var sound = document.getElementById("yippey-sound");
                sound.play();
            }
        </script>
    </body>
</html>
