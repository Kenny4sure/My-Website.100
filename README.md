<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="description" content="Attractive and professional website">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Kehinde Omokanye</title>
    <style>
        body {
            margin: 0;
            font-family: 'Segoe UI', sans-serif;
            background-color: #111;
            color: #fff;
        }

        header {
            background: linear-gradient(90deg, #bfa200, #ffd700);
            padding: 20px;
            text-align: center;
            color: #000;
        }

        h1 {
            margin: 10px 0;
        }

        nav ul {
            list-style: none;
            padding: 0;
            margin: 0;
            display: flex;
            justify-content: center;
            gap: 20px;
        }

        nav ul li a {
            text-decoration: none;
            color: #fff;
            background-color: #bfa200;
            padding: 10px 15px;
            border-radius: 5px;
            transition: 0.3s;
        }

        nav ul li a:hover {
            background-color: #ffd700;
            color: #000;
        }

        section {
            padding: 40px 20px;
            max-width: 900px;
            margin: auto;
            opacity: 0;
            transform: translateY(20px);
            transition: all 1s ease;
        }

        section.show {
            opacity: 1;
            transform: translateY(0);
        }

        footer {
            background-color: #222;
            text-align: center;
            padding: 20px;
            color: #ccc;
        }

        form input, form textarea, form button {
            display: block;
            width: 100%;
            margin: 10px 0;
            padding: 10px;
            font-size: 16px;
        }

        .success-message {
            display: none;
            background-color: green;
            color: white;
            padding: 10px;
            border-radius: 4px;
            margin-top: 10px;
        }
    </style>
</head>
<body>

<header>
    <h1>Kehinde Omokanye</h1>
    <p>Web Developer | UI/UX Designer</p>
</header>

<section id="about">
    <h2>About Me</h2>
    <p>I am Kehinde Omokanye, a creative Web Developer and UI/UX Designer with a passion for building stunning digital experiences.</p>
</section>
<div>
                <nav>
                    <ul class= "nav-links">                        <li><a href="dex.html">About</a></li>
                        </div>
                        <div>
                        <li><a href="Project 1.html">Project 1</a></li>
                        </div>
                        <div>
                        <li><a href="Portfolio II.html">Project 2 </a></li>
                        </div>          
<section id="contact">
    <h2>Contact Me</h2>
    <form id="contactForm">
        <input type="text" name="name" placeholder="Your Name" required />
        <input type="email" name="email" placeholder="Your Email" required />
        <textarea name="message" rows="5" placeholder="Your Message" required></textarea>
        <button type="submit">Send Message</button>
    </form>
    <div class="success-message" id="successMessage">Message successfully sent!</div>
</section>

<footer>
    <p>Kenny Web Design &copy; 2025</p>
</footer>

<script>
    // Show slide animation on scroll
    const sections = document.querySelectorAll('section');

    const revealOnScroll = () => {
        sections.forEach(section => {
            const rect = section.getBoundingClientRect();
            if (rect.top < window.innerHeight - 100) {
                section.classList.add('show');
            }
        });
    };

    window.addEventListener('scroll', revealOnScroll);
    window.addEventListener('load', revealOnScroll);

    // Contact form submission message
    const form = document.getElementById('contactForm');
    const successMessage = document.getElementById('successMessage');

    form.addEventListener('submit', function(e) {
        e.preventDefault();
        successMessage.style.display = 'block';
        form.reset();
    });
</script>
<a href="https://github.com/Kenny4sure/repo.git">GitHub</a>
</body>
</html
