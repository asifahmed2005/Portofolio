<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Asif Ahmed | Portfolio</title>

    <!-- Google Font -->
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600&display=swap" rel="stylesheet">

    <style>
        body {
            margin: 0;
            font-family: "Poppins", sans-serif;
            background: linear-gradient(135deg, #1e1e2f, #232343, #1b1b2b);
            background-size: 400% 400%;
            animation: gradientMove 12s ease infinite;
            color: white;
            overflow-x: hidden;
        }

        @keyframes gradientMove {
            0% { background-position: 0% 50%; }
            50% { background-position: 100% 50%; }
            100% { background-position: 0% 50%; }
        }

        .container {
            width: 85%;
            margin: auto;
            padding: 50px 0;
        }

        /* TYPING ANIMATION */
        .typing {
            font-size: 3rem;
            text-align: center;
            margin-bottom: 20px;
            white-space: nowrap;
            border-right: 3px solid #fff;
            width: 0;
            overflow: hidden;
            margin: auto;
            animation: typing 3s steps(30) forwards, blink .7s infinite;
        }

        @keyframes typing {
            from { width: 0; }
            to { width: 100%; }
        }

        @keyframes blink {
            50% { border-color: transparent; }
        }

        h2 {
            border-left: 5px solid #6c63ff;
            padding-left: 12px;
            font-size: 1.8rem;
        }

        /* 3D CARD EFFECT */
        .card {
            background: rgba(255, 255, 255, 0.08);
            padding: 20px;
            margin: 20px 0;
            border-radius: 12px;
            backdrop-filter: blur(10px);
            transition: transform 0.4s ease, box-shadow 0.4s ease;
            animation: slideUp 1s ease forwards;
            opacity: 0;
            transform-style: preserve-3d;
        }

        .card:nth-child(2) { animation-delay: 0.3s; }
        .card:nth-child(3) { animation-delay: 0.6s; }
        .card:nth-child(4) { animation-delay: 0.9s; }
        .card:nth-child(5) { animation-delay: 1.2s; }

        @keyframes slideUp {
            from { transform: translateY(30px); opacity: 0; }
            to { transform: translateY(0); opacity: 1; }
        }

        /* 3D HOVER */
        .card:hover {
            transform: translateY(-10px) rotateX(8deg) rotateY(8deg) scale(1.05);
            box-shadow: 0 20px 40px rgba(108, 99, 255, 0.5);
        }

        ul {
            padding-left: 20px;
        }

        footer {
            text-align: center;
            margin-top: 40px;
            font-size: 0.9rem;
            opacity: 0.7;
            animation: fadeIn 2s ease forwards;
        }

        a {
            color: #9fa8ff;
            text-decoration: none;
        }
    </style>
</head>

<body>
    <div class="container">

        <!-- TYPING NAME -->
        <div class="typing">👋 Hi, I'm Asif Ahmed</div>

        <div class="card">
            <h2>💡 About Me</h2>
            <p>
                I’m a passionate learner who loves exploring technology, improving myself, 
                and building cool things that make life easier.
            </p>
        </div>

        <div class="card">
            <h2>🚀 What I Am Doing</h2>
            <ul>
                <li>Learning and improving my coding skills</li>
                <li>Exploring web development</li>
                <li>Building small projects for my portfolio</li>
                <li>Learning new tools and productivity methods</li>
            </ul>
        </div>

        <div class="card">
            <h2>🛠️ Skills</h2>
            <ul>
                <li>HTML & CSS (Basic)</li>
                <li>JavaScript (Learning)</li>
                <li>Git & GitHub</li>
                <li>UI/UX basics</li>
                <li>Problem-solving</li>
                <li>Fast learning & adaptability</li>
            </ul>
        </div>

        <div class="card">
            <h2>🎯 Hobbies</h2>
            <ul>
                <li>Gaming</li>
                <li>Watching anime & movies</li>
                <li>Exploring tech</li>
                <li>Photography & editing</li>
                <li>Fitness & self-improvement</li>
            </ul>
        </div>

        <footer>
            Made with ❤️ by Asif Ahmed | 
            <a href="https://github.com/">GitHub Profile</a>
        </footer>
    </div>
</body>
</html>
