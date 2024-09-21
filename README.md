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
            button:hover {
                background-color: limegreen;
            }
        </style>
    </head>
        <h2>welcome to my website!</h2>
        <h2>about me</h2>
        <p>beginner programmer, currently learning python</p>
    <p>games i like, ultrakill, mc, roadblocks</p>
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
        <img src="😴.jpeg" alt="Sleeping Cat" width="250">
    </body>
</html>
<html>
<head>
    <meta charset="utf-8">
    <title>Current Time in Sydney</title>
    <link href="https://fonts.googleapis.com/css2?family=Open+Sans:wght@400;600&display=swap" rel="stylesheet">
    <style>
        body {
            font-family: 'Open Sans', sans-serif;
            margin: 20px;
        }
        #time {
            font-size: 24px;
            margin-top: 20px;
            font-weight: 600;
        }
    </style>
</head>
<body>
      <h2>the time in my city</h2>
    <div class="time-container">
        <p>Current time in Sydney: </p>
        <img src="he IS listening_!__!!_.jpeg" alt="Profile Image" width="20" class="time-image">
    </div>
    <div id="time"></div>

   <script>
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
</html>
