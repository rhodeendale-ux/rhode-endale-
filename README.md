<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Rhode Endale</title>
    <style>
        /* RESET */
        * { margin: 0; padding: 0; box-sizing: border-box; font-family: Arial, sans-serif; }

        body { background: #000; color: #ffd700; line-height: 1.6; scroll-behavior: smooth; }

        /* NAVBAR */
        nav { display: flex; justify-content: space-between; align-items: center; padding: 1rem 2rem; background: #111; position: sticky; top: 0; z-index: 100; }
        nav .logo { font-size: 1.7rem; font-weight: bold; color: #ffd700; }
        nav ul { display: flex; list-style: none; }
        nav ul li { margin-left: 1.5rem; }
        nav ul li a { text-decoration: none; color: #ffd700; font-weight: bold; transition: 0.3s; position: relative; }
        nav ul li a::after { content: ''; display: block; height: 2px; width: 0; background: #fff; transition: 0.3s; position: absolute; bottom: -5px; left: 0; }
        nav ul li a:hover::after { width: 100%; }
        nav ul li a:hover { color: #fff; }

        /* HERO */
        .hero { height: 90vh; display: flex; flex-direction: column; align-items: center; justify-content: center; text-align: center; background: linear-gradient(rgba(0,0,0,0.7), rgba(0,0,0,0.7)), url('https://picsum.photos/1200/800') no-repeat center center/cover; }
        .hero h1 { font-size: 3rem; margin-bottom: 1rem; animation: slideDown 1s ease-out; }
        .hero p { font-size: 1.5rem; margin-bottom: 2rem; animation: slideUp 1s ease-out; }
        .btn { padding: 0.7rem 1.5rem; background: #ffd700; color: #000; font-weight: bold; text-decoration: none; border-radius: 5px; transition: 0.3s; }
        .btn:hover { background: #fff; }

        /* SECTIONS */
        section { padding: 4rem 2rem; }
        .container { max-width: 1000px; margin: 0 auto; }

        /* ABOUT */
        .about p { font-size: 1.2rem; margin-bottom: 2rem; }
        .personal-info p { margin-bottom: 0.5rem; }

        /* SKILLS */
        .skills ul { list-style: none; display: flex; flex-wrap: wrap; gap: 1rem; }
        .skills li { background: #111; padding: 1rem 1.5rem; border-radius: 10px; transition: 0.3s; }
        .skills li:hover { background: #ffd700; color: #000; }

        /* PROJECTS */
        .project-list { display: flex; flex-wrap: wrap; gap: 1rem; justify-content: center; }
        .project-card { background: #111; padding: 1rem; border-radius: 10px; width: 250px; transition: 0.3s; }
        .project-card:hover { transform: scale(1.05); box-shadow: 0 0 20px #ffd700; }

        /* BLOG */
        .blog-post { background: #111; padding: 1rem; border-radius: 10px; margin-bottom: 1rem; transition: 0.3s; }
        .blog-post:hover { box-shadow: 0 0 15px #ffd700; }

        /* CONTACT */
        form { display: flex; flex-direction: column; gap: 1rem; max-width: 500px; margin: 0 auto; }
        input, textarea { padding: 0.7rem; border-radius: 5px; border: none; }
        button { padding: 0.7rem; border-radius: 5px; border: none; background: #ffd700; font-weight: bold; cursor: pointer; transition: 0.3s; }
        button:hover { background: #fff; }

        /* GALLERY */
        .gallery { display: flex; justify-content: center; gap: 1rem; flex-wrap: wrap; margin-top: 2rem; }
        .gallery img { width: 250px; border-radius: 10px; transition: transform 0.5s, box-shadow 0.5s; }
        .gallery img:hover { transform: scale(1.1); box-shadow: 0 0 20px #ffd700; }

        /* ANIMATION */
        @keyframes slideDown { 0% { opacity: 0; transform: translateY(-50px);} 100% { opacity: 1; transform: translateY(0);} }
        @keyframes slideUp { 0% { opacity: 0; transform: translateY(50px);} 100% { opacity: 1; transform: translateY(0);} }
    </style>
</head>
<body>
    <!-- NAVBAR -->
    <nav>
        <div class="logo">Rhode</div>
        <ul>
            <li><a href="#home">Home</a></li>
            <li><a href="#about">About</a></li>
            <li><a href="#skills">Skills</a></li>
            <li><a href="#projects">Projects</a></li>
            <li><a href="#blog">Blog</a></li>
            <li><a href="#contact">Contact</a></li>
        </ul>
    </nav>

    <!-- HERO -->
    <header class="hero" id="home">
        <h1>Hello, I'm Rhode Endale</h1>
        <p>Grade 12 student | Lover of movies, crafts & creativity</p>
        <a href="#about" class="btn">Learn More</a>
    </header>

    <!-- ABOUT -->
    <section class="about" id="about">
        <div class="container">
            <h1>About Me</h1>
            <p>Hi! I'm Rhode Endale, a Grade 12 student. I love eating, watching movies, and doing crafts. I am passionate about learning new skills and creating fun projects.</p>
            <div class="personal-info">
                <p><strong>Email:</strong> rhodeendale@gmail.com</p>
                <p><strong>GitHub:</strong> rhodeendale-ux</p>
                <p><strong>Instagram:</strong> eleanor2.13</p>
                <p><strong>Telegram:</strong> rhode513</p>
            </div>
        </div>
    </section>

    <!-- SKILLS -->
    <section class="skills" id="skills">
        <div class="container">
            <h1>My Skills</h1>
            <ul>
                <li>Web Development (HTML, CSS, JS)</li>
                <li>Graphic Design / Crafts</li>
                <li>Content Creation</li>
                <li>Movie Analysis / Reviews</li>
            </ul>
        </div>
    </section>

    <!-- PROJECTS -->
    <section class="projects" id="projects">
        <div class="container">
            <h1>My Projects</h1>
            <div class="project-list">
                <div class="project-card">
                    <h2>Project 1</h2>
                    <p>Short description of the project. You can add images too!</p>
                </div>
                <div class="project-card">
                    <h2>Project 2</h2>
                    <p>Short description of the project. You can add images too!</p>
                </div>
                <div class="project-card">
                    <h2>Project 3</h2>
                    <p>Short description of the project. You can add images too!</p>
                </div>
            </div>
        </div>
    </section>

    <!-- BLOG -->
    <section class="blog" id="blog">
        <div class="container">
            <h1>My Blog</h1>
            <div class="blog-post">
                <h2>Post 1 Title</h2>
                <p>Some interesting text about your thoughts, movies, crafts, or anything you like.</p>
            </div>
            <div class="blog-post">
                <h2>Post 2 Title</h2>
                <p>Some interesting text about your thoughts, movies, crafts, or anything you like.</p>
            </div>
        </div>
    </section>

    <!-- CONTACT -->
    <section class="contact" id="contact">
        <div class="container">
            <h1>Contact Me</h1>
            <form>
                <input type="text" placeholder="Your Name" required>
                <input type="email" placeholder="Your Email" required>
                <textarea placeholder="Your Message" required></textarea>
                <button type="submit">Send Message</button>
            </form>
        </div>
    </section>

    <!-- GALLERY -->
    <section class="gallery">
        <img src="https://picsum.photos/300/200?1" alt="Pic 1">
        <img src="https://picsum.photos/300/200?2" alt="Pic 2">
        <img src="https://picsum.photos/300/200?3" alt="Pic 3">
    </section>

    <script>
        // Floating gallery images animation
        const images = document.querySelectorAll('.gallery img');
        images.forEach((img, i) => {
            let direction = i % 2 === 0 ? 1 : -1;
            setInterval(() => {
                img.style.transform = `translateY(${10*direction}px)`;
                direction *= -1;
            }, 1500);
        });
    </script>
</body>
</html>
