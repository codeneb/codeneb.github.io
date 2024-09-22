<html>
<head>
    <meta charset="utf-8">
    <title>koneb's devpage</title>
    <link href="https://fonts.googleapis.com/css2?family=Open+Sans:wght@400;600&display=swap" rel="stylesheet">
    <style>
        body {
            font-family: 'Open Sans', sans-serif;
            max-width: 1000px;
            margin-left: auto;
            margin-right: auto;
            padding: 20px; /* Add some padding around the content */
            line-height: 1.6; /* Improves readability by increasing line height */
        }
        h2 {
            margin-top: 40px; /* Adds space before each section header */
        }
        p {
            margin-bottom: 20px; /* Space between paragraphs */
        }
        button {
            background-color: lightgreen;
            color: darkgreen;
            border: none;
            padding: 15px 30px;
            font-size: 18px;
            cursor: pointer;
            border-radius: 5px;
            font-family: 'Open Sans', sans-serif;
            font-weight: 600;
            margin-top: 20px; /* Adds space above the button */
        }
        button:hover {
            background-color: limegreen;
        }
        .time-container {
            display: flex;
            align-items: center;
            margin-top: 30px; /* Adds space above time display */
        }
        img {
            display: block;
            margin-bottom: 40px; /* Adds space below each image */
            max-width: 100%; /* Ensure images are responsive */
        }
        img.time-image {
            margin-right: 10px; /* Space between the time image and text */
        }
        #time {
            font-size: 28px;
            font-weight: 600;
            margin-top: 20px;
        }
    
</head>
<body>
    <h2>welcome to my website!</h2>
    <h2>about me</h2>
    <p>Beginner programmer, currently learning Python.</p>
    <p>Games I like: Ultrakill, Minecraft, Roblox.</p>
 
</head>
<body>
    <h2>Funy button</h2>
    <button onclick="playSound()">Yippey!</button>
    <audio id="yippey-sound">
        <source src="yippee-made-with-Voicemod.mp3" type="audio/mpeg">
        Your browser does not support the audio element.
    </audio>
 
</head>
<body>
    <h2>silly cat images</h2>
    <img src="download (27).jpeg" alt="Profile Image" width="300">
    <img src="😴.jpeg" alt="Sleeping Cat" width="250">
 
</head>
<body>
    <h2>the time in my city</h2>
    <div class="time-container">
        <p>current time in sydney: </p>
        <img src="he IS listening_!__!!_.jpeg" alt="Clock Icon" width="40" class="time-image">
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
</html>
