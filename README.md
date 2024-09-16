
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>My GitHub Portfolio</title>
    <style>
        /* Apply a background image with an animated gradient overlay */
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-image: url('"F:\sublime\1619644762_github-desktop_story.jpg"'); /* Background image from your GitHub */
            background-size: cover;
            background-position: center;
            background-repeat: no-repeat;
            height: 100vh;
            color: white;
            display: flex;
            flex-direction: column;
            justify-content: space-between;
            position: relative;
            overflow: hidden;
        }

        /* Add a subtle animated gradient overlay */
        body::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: linear-gradient(135deg, rgba(0,0,0,0.7), rgba(0,0,0,0.4));
            background-size: 400% 400%;
            animation: gradientAnimation 15s ease infinite;
            z-index: 1; /* Overlay is behind the content */
        }

        /* Gradient animation */
        @keyframes gradientAnimation {
            0% { background-position: 0% 50%; }
            50% { background-position: 100% 50%; }
            100% { background-position: 0% 50%; }
        }

        /* Center the content */
        .container {
            flex: 1; /* Pushes footer to the bottom */
            display: flex;
            justify-content: center;
            align-items: center;
            text-align: center;
            z-index: 2; /* Content stays on top */
        }

        /* Style for the portfolio content */
        .portfolio {
            padding: 20px;
            background: rgba(0, 0, 0, 0.5); /* Semi-transparent background for readability */
            border-radius: 10px;
        }

        h1 {
            font-size: 3em;
            margin: 0;
        }

        p {
            font-size: 1.2em;
            color: white;
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

        /* Icon and buttons at the footer */
        .footer {
            display: flex;
            justify-content: center;
            align-items: center;
            padding: 20px;
            gap: 20px;
            background-color: rgba(0, 0, 0, 0.7); /* Darken the footer for readability */
            z-index: 2; /* Ensure it's above the animation */
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
    </div>

    <!-- Align buttons and icon at the footer -->
    <div class="footer">
        <!-- Download Resume Button -->
        <a href="https://raw.githubusercontent.com/vaish1710/CS620/main/Resume.pdf" class="btn" download="Vaishnavi_Resume.pdf">Download Resume</a>

        <!-- Email Icon Button -->
        <div class="icon">
            <a href="mailto:vaish.paruchuri@gmail.com?subject=Portfolio Inquiry">
                <img src="https://cdn.pixabay.com/photo/2016/06/13/17/30/mail-1454733_640.png" alt="Email Icon" />
            </a>
        </div>
    </div>
</body>
</html>
