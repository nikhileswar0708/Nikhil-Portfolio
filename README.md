<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Nikhileswar Reddy | Portfolio</title>
  <link href="https://unpkg.com/aos@2.3.1/dist/aos.css" rel="stylesheet">
  <style>
    :root {
      --primary: #0f2027;
      --accent: #ffca28;
      --light-bg: #1a1a2e;
    }

    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      font-family: 'Segoe UI', sans-serif;
      background: var(--light-bg);
      color: #f5f5f5;
      scroll-behavior: smooth;
      overflow-x: hidden;
      position: relative;
    }

    nav {
      position: fixed;
      top: 0;
      width: 100%;
      background: rgba(15, 32, 39, 0.95);
      display: flex;
      justify-content: center;
      gap: 2rem;
      padding: 1rem 0;
      z-index: 10;
    }

    nav button {
      background: var(--accent);
      color: #000;
      font-weight: bold;
      padding: 10px 20px;
      border: none;
      border-radius: 25px;
      cursor: pointer;
      transition: background 0.3s;
    }

    nav button:hover {
      background: #e6b800;
    }
    .hero {
      background: linear-gradient(120deg, #0f2027, #203a43, #2c5364);
      color: #fff;
      text-align: center;
      padding: 160px 20px 120px; /* top padding increased */
    }


    .spotlight {
      position: fixed;
      top: 0;
      left: 0;
      width: 100vw;
      height: 100vh;
      pointer-events: none;
      background: radial-gradient(circle at center, rgba(255, 255, 255, 0.1) 0%, transparent 60%);
      z-index: 0;
    }

    .container {
      width: 90%;
      max-width: 1000px;
      margin: auto;
      padding: 2rem 0;
      position: relative;
      z-index: 1;
    }

    .hero {
      background: linear-gradient(120deg, #0f2027, #203a43, #2c5364);
      color: #fff;
      text-align: center;
      padding: 160px 20px 120px; /* extra padding top for nav */
    }
    section {
      scroll-margin-top: 50px; /* Adjust depending on nav height */
    }


    .hero .highlight {
      color: var(--accent);
    }

    .btn {
      display: inline-block;
      margin-top: 20px;
      padding: 12px 25px;
      background: var(--accent);
      color: #000;
      text-decoration: none;
      font-weight: bold;
      border-radius: 30px;
      transition: all 0.3s ease;
    }

    .btn:hover {
      background: #e6b800;
    }

    section h2 {
      font-size: 2.2rem;
      margin-bottom: 1rem;
      color: var(--accent);
    }

    section {
      padding: 4rem 0;
    }

    .about, .skills, .projects, .contact {
      background: #121212;
      border-radius: 12px;
      box-shadow: 0 4px 20px rgba(0, 0, 0, 0.4);
      padding: 2rem;
      margin-bottom: 2rem;
    }

    .skill-list {
      display: flex;
      flex-wrap: wrap;
      gap: 1rem;
      list-style: none;
    }

    .skill-list li {
      background: #2c2c54;
      padding: 10px 20px;
      border-radius: 30px;
      font-weight: bold;
      color: #fff;
    }

    .project-item {
      margin-bottom: 1.5rem;
    }

    form {
      display: flex;
      flex-direction: column;
      gap: 1rem;
    }

    form input, form textarea {
      padding: 12px;
      border: none;
      border-radius: 8px;
      font-size: 1rem;
      background-color: #222;
      color: #fff;
    }

    form button {
      width: fit-content;
    }

    footer {
      background: #000;
      color: #fff;
      text-align: center;
      padding: 1rem;
    }
  </style>
</head>
<body>
  <div class="spotlight" id="spotlight"></div>

  <!-- Navigation Bar -->
<nav>
  <button onclick="document.getElementById('about').scrollIntoView({ behavior: 'smooth' })">About Me</button>
  <button onclick="document.getElementById('skills').scrollIntoView({ behavior: 'smooth' })">Skills</button>
  <button onclick="document.getElementById('projects').scrollIntoView({ behavior: 'smooth' })">Projects</button>
  <button onclick="document.getElementById('contact').scrollIntoView({ behavior: 'smooth' })">Contact Me</button>
  <!--<a href="contact.html"><button>Contact Me</button></a>-->
</nav>



  <!-- Hero Section -->
  <section class="hero" id="home">
    <div class="container">
      <h1>Hello, I'm <span class="highlight">Nikhileswar Reddy</span></h1>
      <p>Software Engineer | App Developer</p>
      <a href="#contact" class="btn">Contact Me</a>
    </div>
  </section>

  <!-- About Section -->
  <section class="about" id="about" data-aos="fade-up">
    <div class="container">
      <h2>About Me</h2>
      <p>
        I'm a Computer Science graduate passionate about software development and building useful applications.
        Skilled in Java, Python, HTML, SQL, and C++. Always eager to learn and collaborate with tech teams to bring ideas to life.
      </p>
    </div>
  </section>

  <!-- Skills Section -->
  <section class="skills" id="skills" data-aos="fade-right">
    <div class="container">
      <h2>Skills</h2>
      <ul class="skill-list">
        <li>Java</li>
        <li>Python</li>
        <li>HTML & CSS</li>
        <li>SQL</li>
        <li>C++</li>

      </ul>
    </div>
  </section>

  <!-- Projects Section -->
  <section class="projects" id="projects" data-aos="zoom-in">
    <div class="container">
      <h2>Projects</h2>
      <div class="project-item">
        <h3>E-Voting System (Blockchain)</h3>
        <p>Developed a tamper-resistant e-voting system using Ethereum blockchain and smart contracts with Truffle and Ganache.</p>
      </div>
      <div class="project-item">
        <h3>Movie Recommendation System</h3>
        <p>Implemented a machine learning model to generate movie suggestions using collaborative filtering and Python.</p>
      </div>
    </div>
  </section>

  <!-- Contact Section -->
  <section class="contact" id="contact" data-aos="flip-up">
    <div class="container">
      <h2>Contact Me</h2>
      <form action="https://formspree.io/f/mnnzzzlo" method="POST">
        <input type="text" name="name" placeholder="Your Name" required />
        <input type="email" name="email" placeholder="Your Email" required />
        <textarea name="message" rows="5" placeholder="Your Message" required></textarea>
        <button type="submit" class="btn">Send Message</button>
      </form>
    </div>
  </section>

  <!-- Footer -->
  <footer>
    <p>© 2025 Nikhileswar Reddy. All Rights Reserved.</p>
  </footer>

  <script src="https://unpkg.com/aos@2.3.1/dist/aos.js"></script>
  <script>
    AOS.init();

    const spotlight = document.getElementById("spotlight");
    let mouseX = 0, mouseY = 0;
    let currentX = 0, currentY = 0;

    document.addEventListener("mousemove", (e) => {
      mouseX = e.clientX;
      mouseY = e.clientY;
    });

    function animateSpotlight() {
      const speed = 0.03;
      currentX += (mouseX - currentX) * speed;
      currentY += (mouseY - currentY) * speed;
      spotlight.style.background = `radial-gradient(circle at ${currentX}px ${currentY}px, rgba(255, 255, 255, 0.1) 0%, transparent 60%)`;
      requestAnimationFrame(animateSpotlight);
    }

    animateSpotlight();
  </script>
</body>
</html>
