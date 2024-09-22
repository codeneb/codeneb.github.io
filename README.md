<html lang="en">
<head>
    <meta charset="utf-8">
    <title>koneb's devpage</title>
    <link href="https://fonts.googleapis.com/css2?family=Open+Sans:wght@400;600&display=swap" rel="stylesheet">
    <style>
        body {
            font-family: 'Open Sans', sans-serif;
            margin: 20px;
            max-width: 1350px; /* Limit the width of the content */
            margin-left: auto; /* Center the container */
            margin-right: auto; /* Center the container */
        }
        h2 {
            margin-top: 60px;
            margin-bottom: 50px;
        }
        p {
            margin-bottom: 20px;
        }
        button {
            background-color: lightgreen;
            color: darkgreen;
            border: none;
            padding: 10px 20px;
            font-size: 16px;
            cursor: pointer;
            border-radius: 5px;
            font-weight: 600;
            margin-bottom: 20px; /* Space below the button */
        }
        button:hover {
            background-color: limegreen;
        }
        #time {
            font-size: 24px;
            margin-top: 20px;
            font-weight: 600;
        }
        .time-container {
            display: flex;
            align-items: center; /* Aligns items vertically centered */
        }
        img {
            display: block; /* Ensures images are block elements */
            margin-bottom: 20px; /* Space below each image */
        }
        img.time-image {
            margin-right: 10px; /* Space between image and text */
        }
    </style>
</head>
<body>
    <h2>welcome to my website!</h2>
    <h2>about me</h2>
    <p>beginner programmer, currently learning Python.</p>
    <p>Games I like: Ultrakill, Minecraft, Roblox.</p>
<body>
    <h2>funny button</h2>
    <button onclick="playSound()">yippey</button>
    <audio id="yippey-sound">
        <source src="yippee-made-with-Voicemod.mp3" type="audio/mpeg">
        Your browser does not support the audio element.
    </audio>
<body>
    <h2>silly cat images</h2>
    <img src="download (27).jpeg" alt="Profile Image" width="300">
    <img src="😴.jpeg" alt="Sleeping Cat" width="450">
    <h2>the time in my city</h2>
    <div class="time-container">
        <p>Current time in Sydney:</p>
        <img src="he IS listening_!__!!_.jpeg" alt="Profile Image" width="50" class="time-image">
    </div>
    <div id="time"></div>
    <script>
        function playSound() {
            var sound = document.getElementById("yippey-sound");
            sound.play();
        }
        function updateTime() {
            const options = { timeZone: 'Australia/Sydney', hour: '2-digit', minute: '2-digit', second: '2-digit' };
            const timeString = new Intl.DateTimeFormat('en-AU', options).format(new Date());
            document.getElementById('time').textContent = timeString;
        }
        // Update the time every second
        setInterval(updateTime, 1000);
        updateTime(); // Initial call to display time immediately
    </script>
</body>

