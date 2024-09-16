
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>My GitHub Portfolio</title>
    <style>
        /* Apply a background image with an animated gradient overlay */
        body {
            font-family: 'Poppins', sans-serif;
            margin: 0;
            padding: 0;
            background-image: url('https://raw.githubusercontent.com/vaish1710/CS620/main/102393310-07478b80-3f8d-11eb-84eb-392d555ebd29.webp'); /* Updated Background Image */
            background-size: cover;
            background-position: center;
            background-repeat: no-repeat;
            height: 100vh;
            color: white;
            display: flex;
            flex-direction: column;
            justify-content: space-between;
            overflow: hidden;
            position: relative;
            scroll-behavior: smooth; /* Smooth scroll for future sections */
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
            z-index: 1;
        }

        /* Gradient animation */
        @keyframes gradientAnimation {
            0% { background-position: 0% 50%; }
            50% { background-position: 100% 50%; }
            100% { background-position: 0% 50%; }
        }

        /* Glow effect for the title */
        h1 {
            font-size: 3em;
            color: #4CAF50;
            text-shadow: 0 0 15px #4CAF50, 0 0 25px #4CAF50, 0 0 40px #4CAF50;
            margin: 0;
        }

        /* Center the content */
        .container {
            flex: 1;
            display: flex;
            justify-content: center;
            align-items: center;
            text-align: center;
            z-index: 2;
        }

        /* Style for the portfolio content */
        .portfolio {
            padding: 30px;
            border-radius: 15px;
            background: rgba(0, 0, 0, 0.5);
            backdrop-filter: blur(5px); /* Blurs the background under the content */
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.3);
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }

        /* Card hover effect */
        .portfolio:hover {
            transform: scale(1.05);
            box-shadow: 0 8px 20px rgba(0, 0, 0, 0.5);
        }

        p {
            font-size: 1.2em;
            color: white;
        }

        a {
            color: #4CAF50;
            text-decoration: none;
            font-weight: bold;
            position: relative;
        }

        a::before {
            content: '';
            position: absolute;
            width: 100%;
            height: 2px;
            bottom: 0;
            left: 0;
            background-color: #4CAF50;
            visibility: hidden;
            transform: scaleX(0);
            transition: all 0.3s ease-in-out;
        }

        a:hover::before {
            visibility: visible;
            transform: scaleX(1);
        }

        /* Button styling with hover effect */
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
            transition: all 0.3s ease;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.3);
        }

        .btn:hover {
            background-color: #45a049;
            transform: translateY(-3px);
            box-shadow: 0 6px 15px rgba(0, 0, 0, 0.5);
        }

        /* Footer with flexbox */
        .footer {
            display: flex;
            justify-content: center;
            align-items: center;
            padding: 20px;
            gap: 20px;
            background-color: rgba(0, 0, 0, 0.8);
            z-index: 2;
        }

        .icon img {
            width: 40px;
            height: 40px;
            cursor: pointer;
            transition: transform 0.3s ease;
        }

        .icon img:hover {
            transform: rotate(15deg);
        }

        /* Animations on scroll for the content */
        .fade-in {
            opacity: 0;
            transform: translateY(50px);
            transition: opacity 0.8s ease, transform 0.8s ease;
        }

        .fade-in.visible {
            opacity: 1;
            transform: translateY(0);
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="portfolio fade-in">
            <h1>Vaishnavi Paruchuri</h1>
            <p>Data Science and Analytics Master's Student</p>
            <p>I hold an undergraduate degree in Computer Science and am currently pursuing a master's in Data Science and Analytics. My primary interest lies in uncovering valuable outcomes from data, driving insights that lead to informed decisions and innovation.</p>
            <p>Check out my repositories on <a href="https://github.com/vaish1710" target="_blank">GitHub</a>.</p>
        </div>
    </div>

    <!-- Footer with buttons and email icon -->
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

    <script>
        /* JavaScript to handle the fade-in animation */
        document.addEventListener("DOMContentLoaded", function() {
            var portfolio = document.querySelector('.portfolio');
            portfolio.classList.add('visible');
        });
    </script>
</body>
</html>
