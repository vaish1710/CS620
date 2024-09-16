
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>My GitHub Portfolio</title>
    <style>
        /* Apply a background image */
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-image: url('"F:\sublime\wy2o6nicut63th7nn6dg.jpg"'); /* Background image from your GitHub */
            background-size: cover; /* Make sure image covers the entire viewport */
            background-position: center;
            background-repeat: no-repeat;
            height: 100vh;
            color: white;
        }

        /* Center the content */
        .container {
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            text-align: center;
        }

        /* Style for the portfolio content */
        .portfolio {
            padding: 20px;
        }

        h1 {
            font-size: 3em;
            margin: 0;
        }

        p {
            font-size: 1.2em;
            color: white; /* Ensure text is visible against the background */
        }

        a {
            color: #4CAF50;
            text-decoration: none;
            font-weight: bold;
        }

        a:hover {
            text-decoration: underline;
        }

        /* Button styling */
        .btn {
            display: inline-block;
            padding: 10px 20px;
            font-size: 1.1em;
            background-color: #4CAF50;
            color: white;
            border: none;
            border-radius: 5px;
            text-decoration: none;
            cursor: pointer;
        }

        .btn:hover {
            background-color: #45a049;
        }

        /* Icon and buttons at the bottom */
        .bottom-buttons {
            position: absolute;
            bottom: 20px;
            left: 50%;
            transform: translateX(-50%);
            display: flex;
            gap: 20px;
        }

        .icon img {
            width: 40px;
            height: 40px;
            cursor: pointer;
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="portfolio">
            <h1>Vaishnavi Paruchuri</h1>
            <p>Data Science and Analytics Master's Student</p>
            <p>I hold an undergraduate degree in Computer Science and am currently pursuing a master's in Data Science and Analytics. My primary interest lies in uncovering valuable outcomes from data, driving insights that lead to informed decisions and innovation.</p>
            <p>Check out my repositories on <a href="https://github.com/vaish1710" target="_blank">GitHub</a>.</p>
        </div>

        <!-- Align buttons and icon at the bottom -->
        <div class="bottom-buttons">
            <!-- Download Resume Button -->
            <a href="https://raw.githubusercontent.com/vaish1710/CS620/main/Resume.pdf" class="btn" download="Vaishnavi_Resume.pdf">Download Resume</a>

            <!-- Email Icon Button -->
            <div class="icon">
                <a href="mailto:vaish.paruchuri@gmail.com?subject=Portfolio Inquiry">
                    <img src="https://cdn.pixabay.com/photo/2016/06/13/17/30/mail-1454733_640.png" alt="Email Icon" />
                </a>
            </div>
        </div>
    </div>
</body>
</html>

