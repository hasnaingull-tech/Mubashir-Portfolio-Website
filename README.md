<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Mubashir Meo | Professional Virtual Assistant & Digital Marketing Specialist</title>

    <!-- Fonts & Icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&family=Montserrat:wght@400;500;600;700&display=swap" rel="stylesheet">

    <style>
        :root {
            --primary: #1a365d;
            --secondary: #f7b731;
            --accent: #2d3748;
            --light: #f8f9fa;
            --dark: #1a202c;
            --text: #4a5568;
            --white: #ffffff;
            --shadow: 0 10px 30px rgba(0,0,0,0.08);
            --radius: 10px;
            --transition: all 0.3s ease;
        }

        * { margin: 0; padding: 0; box-sizing: border-box; }
        body {
            font-family: 'Poppins', sans-serif;
            background: var(--light);
            color: var(--text);
            line-height: 1.6;
        }

        h1,h2,h3,h4 { font-family: 'Montserrat', sans-serif; }
        img { max-width: 100%; }

        .container {
            width: 90%;
            max-width: 1200px;
            margin: auto;
        }

        section { padding: 100px 0; }

        /* Header */
        header {
            position: fixed;
            width: 100%;
            background: var(--white);
            box-shadow: var(--shadow);
            z-index: 1000;
        }

        .navbar {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 20px 0;
        }

        .logo {
            font-size: 1.8rem;
            font-weight: 700;
            color: var(--primary);
        }

        .logo span { color: var(--secondary); }

        .nav-menu {
            display: flex;
            list-style: none;
        }

        .nav-item { margin-left: 30px; }

        .nav-link {
            text-decoration: none;
            color: var(--dark);
            font-weight: 500;
        }

        .nav-link:hover { color: var(--secondary); }

        .hamburger {
            display: none;
            font-size: 1.8rem;
            cursor: pointer;
        }

        /* Hero */
        .hero {
            background: linear-gradient(rgba(26,54,93,.9), rgba(26,54,93,.9)),
            url('https://images.unsplash.com/photo-1522071820081-009f0129c71c') center/cover;
            color: white;
            text-align: center;
            padding: 180px 0 120px;
        }

        .hero h1 { font-size: 3rem; margin-bottom: 20px; }
        .hero p { max-width: 700px; margin: auto auto 30px; }

        .btn {
            background: var(--secondary);
            padding: 14px 30px;
            border-radius: var(--radius);
            text-decoration: none;
            color: var(--dark);
            font-weight: 600;
            margin: 5px;
            display: inline-block;
        }

        .btn-outline {
            background: transparent;
            border: 2px solid white;
            color: white;
        }

        /* About */
        .about {
            background: white;
        }

        .about-content {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 60px;
            align-items: center;
        }

        /* Skills, Services, Cards */
        .card {
            background: white;
            padding: 30px;
            border-radius: var(--radius);
            box-shadow: var(--shadow);
            text-align: center;
        }

        /* Contact */
        .contact-container {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 50px;
        }

        input, textarea {
            width: 100%;
            padding: 15px;
            border-radius: var(--radius);
            border: 1px solid #ddd;
            margin-bottom: 15px;
            font-family: inherit;
        }

        /* Footer */
        footer {
            background: var(--primary);
            color: white;
            padding: 60px 0 20px;
        }

        .social-icons a {
            color: white;
            margin-right: 15px;
            font-size: 1.2rem;
        }

        /* Responsive */
        @media (max-width: 768px) {
            .about-content,
            .contact-container {
                grid-template-columns: 1fr;
            }
            .nav-menu {
                display: none;
                flex-direction: column;
                background: white;
                width: 100%;
                position: absolute;
                top: 70px;
                left: 0;
            }
            .nav-menu.active { display: flex; }
            .hamburger { display: block; }
        }
    </style>
</head>

<body>

<header>
    <div class="container">
        <nav class="navbar">
            <div class="logo">Mubashir<span>Meo</span></div>
            <ul class="nav-menu">
                <li class="nav-item"><a href="#home" class="nav-link">Home</a></li>
                <li class="nav-item"><a href="#about" class="nav-link">About</a></li>
                <li class="nav-item"><a href="#skills" class="nav-link">Skills</a></li>
                <li class="nav-item"><a href="#services" class="nav-link">Services</a></li>
                <li class="nav-item"><a href="#contact" class="nav-link">Contact</a></li>
            </ul>
            <div class="hamburger"><i class="fas fa-bars"></i></div>
        </nav>
    </div>
</header>

<section id="home" class="hero">
    <div class="container">
        <h1>Mubashir Meo</h1>
        <p>Professional Virtual Assistant & Digital Marketing Specialist</p>
        <a href="#contact" class="btn">Get In Touch</a>
        <a href="#services" class="btn btn-outline">View Services</a>
    </div>
</section>

<section id="about" class="about">
    <div class="container">
        <div class="about-content">
            <img src="https://images.unsplash.com/photo-1507003211169-0a1dd7228f2d" alt="Profile">
            <div>
                <h2>About Me</h2>
                <p>I help businesses grow through Amazon management, digital marketing, and professional virtual assistance.</p>
            </div>
        </div>
    </div>
</section>

<section id="contact">
    <div class="container">
        <h2>Contact Me</h2>
        <div class="contact-container">
            <div>
                <p>Email: contact@mubashirmeo.com</p>
                <p>WhatsApp: +1 (123) 456-7890</p>
            </div>
            <form id="contactForm">
                <input type="text" placeholder="Your Name" required>
                <input type="email" placeholder="Your Email" required>
                <textarea placeholder="Your Message" required></textarea>
                <button class="btn" type="submit">Send</button>
            </form>
        </div>
    </div>
</section>

<footer>
    <div class="container">
        <p>&copy; 2023 Mubashir Meo</p>
        <div class="social-icons">
            <a href="#"><i class="fab fa-linkedin"></i></a>
            <a href="#"><i class="fab fa-facebook"></i></a>
            <a href="#"><i class="fab fa-whatsapp"></i></a>
        </div>
    </div>
</footer>

<script>
    const hamburger = document.querySelector('.hamburger');
    const menu = document.querySelector('.nav-menu');

    hamburger.onclick = () => menu.classList.toggle('active');

    document.getElementById('contactForm').onsubmit = e => {
        e.preventDefault();
        alert("Message sent successfully!");
        e.target.reset();
    };
</script>

</body>
</html>
