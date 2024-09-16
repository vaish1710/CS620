
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
            background-image: url('https://raw.githubusercontent.com/vaish1710/CS620/main/102393310-07478b80-3f8d-11eb-84eb-392d555ebd29.webp');
            background-size: cover; /* Ensures the image covers the entire viewport */
            background-position: center;
            background-repeat: no-repeat;
            height: 100vh; /* Ensures the body takes the full viewport height */
            color: white;
        }

        /* Center the content */
        .container {
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            text-align: center;
            background-color: rgba(0, 0, 0, 0.6); /* Darken the background for readability */
            position: relative;
        }

        /* Style for the portfolio content */
        .portfolio {
            padding: 20px;
            border-radius: 15px;
            background-color: rgba(0, 0, 0, 0); /* Transparent background */
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            box-shadow: none !important; /* Force removal of box shadow */
            border: none; /* Ensure no border is applied */
        }

        /* Style for the name */
        h1 {
            font-size: 7em; /* Increase font size */
            margin: 0;
            font-weight: bold;
            text-decoration: none; /* Ensure no underline */
        }

        /* Remove underline from the name if it’s a link */
        h1 a {
            text-decoration: none; /* Ensure no underline for links within h1 */
        }

        p {
            font-size: 1.2em;
            margin: 15px 0;
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
            padding: 12px 30px; /* Adjusted padding */
            font-size: 1.1em;
            background-color: #4CAF50;
            color: white;
            border: none;
            border-radius: 3px; /* Reduced corner radius */
            box-shadow: 0px 4px 6px rgba(0, 0, 0, 0.2); /* Add subtle shadow */
            text-decoration: none;
            cursor: pointer;
            transition: background-color 0.3s ease, box-shadow 0.3s ease;
        }

        .btn:hover {
            background-color: #45a049;
            box-shadow: 0px 4px 6px rgba(0, 0, 0, 0.4); /* Darker shadow on hover */
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

        /* Styling for the mail icon */
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
