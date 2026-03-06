<!DOCTYPE html>                                                        
<html lang="en">                                            
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>My First Website</title>
  
  <style>
    * {
      margin: 0;                                                   
      padding: 0;
      box-sizing: border-box;
    }

    html {
      scroll-behavior: smooth;
    }

    body {
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      line-height: 1.6;
      color: #333;
      background-color: #f9f9f9;
    }

    header {
      background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
      color: white;
      padding: 1rem 0;
      position: sticky;
      top: 0;
      z-index: 100;
      box-shadow: 0 2px 10px rgba(0,0,0,0.15);
    }

    nav {
      max-width: 1200px;
      margin: 0 auto;
      padding: 0 2rem;
      display: flex;
      justify-content: space-between;
      align-items: center;
    }

    .logo {
      font-size: 1.8rem;
      font-weight: bold;
    }

    .nav-links a {
      color: white;
      text-decoration: none;
      margin-left: 2rem;
      font-weight: 500;
      transition: color 0.3s;
    }

    .nav-links a:hover {
      color: #ffe066;
    }

    .hero {
      background: linear-gradient(rgba(0,0,0,0.5), rgba(0,0,0,0.7)),
                  url('https://images.unsplash.com/photo-1557683316-973673baf926?auto=format&fit=crop&w=1350&q=80');
      background-size: cover;
      background-position: center;
      color: white;
      text-align: center;
      padding: 14rem 2rem 10rem;
    }

    .hero h1 {
      font-size: 3.8rem;
      margin-bottom: 1.2rem;
      text-shadow: 2px 2px 12px rgba(0,0,0,0.7);
    }

    .hero p {
      font-size: 1.5rem;
      max-width: 720px;
      margin: 0 auto 2.5rem;
    }

    .btn {
      display: inline-block;
      background-color: #ffe066;
      color: #222;
      padding: 1rem 2.5rem;
      text-decoration: none;
      border-radius: 50px;
      font-weight: bold;
      transition: all 0.3s;
    }

    .btn:hover {
      background-color: #ffd633;
      transform: translateY(-4px);
      box-shadow: 0 10px 25px rgba(0,0,0,0.25);
    }

    main {
      max-width: 1100px;
      margin: 5rem auto;
      padding: 0 2rem;
    }

    section {
      margin-bottom: 7rem;
    }

    h2 {
      color: #4a4a8c;
      text-align: center;
      margin-bottom: 3rem;
      font-size: 2.6rem;
      position: relative;
    }

    h2::after {
      content: '';
      width: 80px;
      height: 4px;
      background: #764ba2;
      position: absolute;
      bottom: -12px;
      left: 50%;
      transform: translateX(-50%);
      border-radius: 2px;
    }

    /* About */
    #about p {
      max-width: 780px;
      margin: 0 auto 2rem;
      font-size: 1.15rem;
      text-align: center;
    }

    /* Services */
    .cards {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
      gap: 2.2rem;
    }

    .card {
      background: white;
      border-radius: 12px;
      overflow: hidden;
      box-shadow: 0 6px 18px rgba(0,0,0,0.09);
      transition: all 0.35s;
    }

    .card:hover {
      transform: translateY(-12px);
      box-shadow: 0 18px 35px rgba(0,0,0,0.18);
    }

    .card img {
      width: 100%;
      height: 210px;
      object-fit: cover;
    }

    .card-content {
      padding: 1.8rem;
      text-align: center;
    }

    .card h3 {
      margin-bottom: 1rem;
      color: #4a4a8c;
    }

    /* Contact */
    #contact {
      background: #f0f0ff;
      padding: 5rem 2rem;
      border-radius: 16px;
    }

    .contact-container {
      max-width: 800px;
      margin: 0 auto;
    }

    form {
      display: grid;
      gap: 1.4rem;
    }

    input, textarea {
      width: 100%;
      padding: 1rem;
      border: 2px solid #ddd;
      border-radius: 8px;
      font-size: 1.05rem;
      transition: border-color 0.3s;
    }

    input:focus, textarea:focus {
      outline: none;
      border-color: #764ba2;
      box-shadow: 0 0 0 3px rgba(118,75,162,0.15);
    }

    textarea {
      min-height: 160px;
      resize: vertical;
    }

    .form-btn {
      background: #764ba2;
      color: white;
      border: none;
      padding: 1rem 2.5rem;
      font-size: 1.1rem;
      border-radius: 50px;
      cursor: pointer;
      transition: all 0.3s;
      justify-self: center;
    }

    .form-btn:hover {
      background: #5a3d8a;
      transform: translateY(-3px);
    }

    footer {
      background: #2d2d44;
      color: #ddd;
      text-align: center;
      padding: 3.5rem 1rem;
      margin-top: 5rem;
    }

    @media (max-width: 768px) {
      .hero { padding: 10rem 1.5rem 7rem; }
      .hero h1 { font-size: 2.8rem; }
      nav { flex-direction: column; gap: 1.2rem; padding: 1.2rem; }
      .nav-links a { margin: 0 1.1rem; font-size: 1.05rem; }
    }
  </style>
</head>
<body>

  <header>
    <nav>
      <div class="logo">Department of Computer Science and Engineering (CSE)</div>
      <div class="nav-links">
        <a href="#home">Home</a>
        <a href="#about">About</a>
        <a href="#services">Services</a>
        <a href="#contact">Contact</a>
      </div>
    </nav>
  </header>

  <section class="hero" id="home">
    <h1>Dept of CSE</h1>
    <p>Computer Science Engineering (CSE) is a premier academic discipline combining computer science and electrical engineering to develop, test, and maintain hardware and software systems. It merges theoretical computation, algorithms, and programming with practical applications in AI, cybersecurity, and data science to solve real-world problems.</p>
    <a href="#contact" class="btn">Get in Touch</a>
  </section>

  <main>
    <section id="about">
      <h2>About Us</h2>
      <p>About the Department of Computer Science and Engineering</p>
      <p>Welcome to the Department of Computer Science and Engineering (CSE) at Swarnandhra College of Engineering and Technology</p>
<p>Established in 2001, the CSE Department has grown into one of the most dynamic and sought-after academic units in the institution. We are committed to excellence in education, research, and innovation, preparing students to thrive in the rapidly evolving world of computing and technology.</p>
<ul style="list-style: none; margin: 2rem 0; padding: 0; display: flex; flex-wrap: wrap; justify-content: center; gap: 1.5rem 2.5rem; font-weight: 500; color: #4a4a8c;">
      <li>Artificial Intelligence & Machine Learning</li>
      <li>Data Science & Big Data Analytics</li>
      <li>Cybersecurity & Network Security</li>
      <li>Cloud Computing & IoT</li>
      <li>Software Engineering & DevOps</li>
      <li>Computer Vision & Robotics</li>
      <li>Blockchain & Distributed Systems</li>
    </ul>
    </section>

    <section id="services">
      <h2>Our Services</h2>
      <div class="cards">
        <div class="card">
          <img src="https://images.unsplash.com/photo-1555066931-bf19c65fd1b4?auto=format&fit=crop&w=800&q=80" alt="Web Development">
          <div class="card-content">
            <h3>Web Development</h3>
            <p>Custom websites, e-commerce stores, web applications, landing pages — built with modern technologies.</p>
          </div>
        </div>
        
        <div class="card">
          <img src="https://images.unsplash.com/photo-1498050108023-c5249f4df085?auto=format&fit=crop&w=800&q=80" alt="UI/UX Design">
          <div class="card-content">
            <h3>UI/UX Design</h3>
            <p>User-centered design, wireframes, prototypes, visual identity and consistent brand experience.</p>
          </div>
        </div>
        
        <div class="card">
          <img src="https://images.unsplash.com/photo-1460925898913-fff696a9d776?auto=format&fit=crop&w=800&q=80" alt="SEO & Marketing">
          <div class="card-content">
            <h3>SEO & Growth</h3>
            <p>Technical SEO, on-page optimization, content strategy and basic digital marketing support.</p>
          </div>
        </div>
      </div>
    </section>

    <section id="contact">
      <h2>Contact Us</h2>
      <div class="contact-container">
        <form action="https://formsubmit.co/your@email.com" method="POST">
          <input type="text" name="name" placeholder="Your Name" required>
          <input type="email" name="email" placeholder="Your Email" required>
          <input type="text" name="subject" placeholder="Subject" required>
          <textarea name="message" placeholder="Your message..." required></textarea>
          <button type="submit" class="form-btn">Send Message</button>
        </form>
      </div>
    </section>
  </main>

  <footer>
    <p>© 2026 MyCompany — All rights reserved.<br>
    Made with passion using only HTML & CSS</p>
  </footer>

</body>
</html>

