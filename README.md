# rizamaerivera.Github.io
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Your Name | Portfolio</title>

    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Poppins', sans-serif;
        }

        body {
            background: linear-gradient(135deg, #0f2027, #203a43, #2c5364);
            color: white;
            scroll-behavior: smooth;
        }

        nav {
            position: fixed;
            width: 100%;
            top: 0;
            background: rgba(0, 0, 0, 0.4);
            padding: 15px;
            text-align: center;
            backdrop-filter: blur(10px);
            z-index: 10;
        }

        nav a {
            color: white;
            margin: 0 15px;
            text-decoration: none;
            font-weight: 500;
        }

        header {
            min-height: 100vh;
            display: flex;
            align-items: center;
            justify-content: center;
            padding: 100px 10%;
        }

        .hero {
            display: flex;
            align-items: center;
            gap: 50px;
            flex-wrap: wrap;
        }

        .hero img {
            width: 250px;
            height: 250px;
            object-fit: cover;
            border-radius: 50%;
            border: 4px solid rgba(255,255,255,0.3);
            box-shadow: 0 0 30px rgba(0, 198, 255, 0.6);
        }

        .hero-text h1 {
            font-size: 3rem;
        }

        .hero-text p {
            font-size: 1.2rem;
            opacity: 0.85;
            margin-top: 10px;
        }

        section {
            padding: 80px 10%;
        }

        h2 {
            font-size: 2.5rem;
            text-align: center;
            margin-bottom: 40px;
        }

        .glass {
            background: rgba(255, 255, 255, 0.1);
            border-radius: 15px;
            padding: 30px;
            backdrop-filter: blur(10px);
            max-width: 900px;
            margin: auto;
        }

        .skill {
            margin-bottom: 20px;
        }

        .bar {
            background: #333;
            border-radius: 20px;
            overflow: hidden;
        }

        .bar span {
            display: block;
            height: 14px;
            width: 0;
            background: linear-gradient(90deg, #00c6ff, #0072ff);
            border-radius: 20px;
            transition: width 2s ease;
        }

        .projects {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 20px;
        }

        .project-card {
            background: rgba(255,255,255,0.1);
            padding: 20px;
            border-radius: 15px;
            transition: transform 0.3s;
        }

        .project-card:hover {
            transform: translateY(-10px);
        }

        footer {
            text-align: center;
            padding: 20px;
            background: rgba(0,0,0,0.4);
        }

        @media (max-width: 768px) {
            .hero {
                justify-content: center;
                text-align: center;
            }
        }
    </style>
</head>
<body>

<nav>
    <a href="#home">Home</a>
    <a href="#about">About</a>
    <a href="#skills">Skills</a>
    <a href="#projects">Projects</a>
    <a href="#contact">Contact</a>
</nav>

<header id="home">
    <div class="hero">
        <a href="https://ibb.co/yn2zGcsZ"><img src="https://i.ibb.co/xSZnPt5B/Screenshot-2026-01-08-21-47-03-18-346179721850c7a35aa3cffbc028dbe4.jpg" alt="Screenshot-2026-01-08-21-47-03-18-346179721850c7a35aa3cffbc028dbe4" border="0"></a>
        <div class="hero-text">
            <h1>Riza Mae Rivera</h1>
            <p>Web Developer | JavaScript Enthusiast</p>
        </div>
    </div>
</header>

<section id="about">
    <h2>About Me</h2>
    <div class="glass">
        <p>
            I am a passionate web developer who enjoys building clean, modern, and responsive websites.
            I love working with HTML, CSS, JavaScript, and continuously improving my skills.
        </p>
    </div>
</section>

<section id="skills">
    <h2>Skills</h2>
    <div class="glass">

        <div class="skill">
            <p>Wattpad</p>
           
        </div>

        <div class="skill">
            <p>Badminton</p>
           
        </div>

        <div class="skill">
            <p>Watching Kdrama</p>
         
        </div>

    </div>
</section>

<section id="projects">
    <h2>Projects</h2>
    <div class="projects glass">
        <div class="project-card">
            <h3>Portfolio Website</h3>
            <p>Personal portfolio built with HTML, CSS, and JavaScript.</p>
        </div>

        <div class="project-card">
            <h3>Todo App</h3>
            <p>A JavaScript-based task management app.</p>
        </div>

        <div class="project-card">
            <h3>Landing Page</h3>
            <p>Responsive product landing page design.</p>
        </div>
    </div>
</section>

<section id="contact">
    <h2>Contact</h2>
    <div class="glass">
        <p>Email: yourname@email.com</p>
        <p>GitHub | LinkedIn | Twitter</p>
    </div>
</section>

<footer>
    <p>© 2026 Your Name. All Rights Reserved.</p>
</footer>

<script>
    // Animate skill bars when visible
    const bars = document.querySelectorAll('.bar span');

    window.addEventListener('scroll', () => {
        bars.forEach(bar => {
            const rect = bar.getBoundingClientRect();
            if (rect.top < window.innerHeight) {
                bar.style.width = bar.dataset.width;
            }
        });
    });
</script>

</body>
</html>
