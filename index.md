---
layout: default
title: "Home"
---

<!-- Custom CSS -->
<link rel="stylesheet" href="{{ '/assets/css/style.css' | relative_url }}">

<!-- Top Navigation -->
<nav class="navbar">
  <div class="nav-inner">
    <a class="brand" href="{{ '/' | relative_url }}">KC</a>
    <div class="links">
      <a href="{{ '/' | relative_url }}">Home</a>
      <a href="{{ '/projects' | relative_url }}">Projects</a>
      <a href="{{ '/contact' | relative_url }}">Contact</a>
    </div>
  </div>
</nav>

<!-- Hero -->
<header class="hero">
  <img src="{{ '/assets/img/profile.jpg' | relative_url }}" alt="Profile photo" class="avatar">
  <h1>Konstantinos Christopoulos</h1>
  <p class="tagline">Computer Engineering & Informatics Graduate — building intelligent systems in <strong>Robotics</strong>, <strong>ML/CV</strong>, and <strong>Full-Stack</strong>.</p>
  <div class="cta">
    <a class="btn primary" href="{{ '/assets/CV_Konstantinos_Christopoulos.pdf' | relative_url }}" target="_blank">Download CV</a>
    <a class="btn" href="https://github.com/YOUR_GITHUB_USERNAME" target="_blank">GitHub</a>
    <a class="btn" href="https://www.linkedin.com/in/YOUR_LINKEDIN" target="_blank">LinkedIn</a>
    <a class="btn ghost" href="mailto:YOUR_EMAIL@example.com">Email me</a>
  </div>

  <div class="badges">
    <img alt="Python" src="https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=white">
    <img alt="ROS" src="https://img.shields.io/badge/ROS-22314E?logo=ros&logoColor=white">
    <img alt="OpenCV" src="https://img.shields.io/badge/OpenCV-5C3EE8?logo=opencv&logoColor=white">
    <img alt="Spring Boot" src="https://img.shields.io/badge/Spring%20Boot-6DB33F?logo=springboot&logoColor=white">
    <img alt="Docker" src="https://img.shields.io/badge/Docker-2496ED?logo=docker&logoColor=white">
    <img alt="Git" src="https://img.shields.io/badge/Git-F05032?logo=git&logoColor=white">
  </div>
</header>

<!-- Featured Projects -->
<section class="section">
  <h2>Featured Projects</h2>

  <div class="cards">
    <article class="card">
      <img src="{{ '/assets/img/jackal_demo.jpg' | relative_url }}" alt="Jackal demo" class="card-img">
      <div class="card-body">
        <h3>Robot Navigation in Crowded Environments</h3>
        <p>Navigation stack for Clearpath <strong>Jackal</strong> with ROS Noetic, LiDAR pedestrian detection (VLP-16), social force models (<em>pedsim_ros</em>), and custom robot avoidance.</p>
        <p class="tech">Python, C++, ROS, Gazebo, OpenCV/YOLO</p>
        <div class="card-actions">
          <a class="btn small" href="https://github.com/YOUR_GITHUB_USERNAME/robot-navigation" target="_blank">Repo</a>
          <a class="btn small ghost" href="https://YOUR_DEMO_LINK" target="_blank">Demo</a>
        </div>
      </div>
    </article>

    <article class="card">
      <img src="{{ '/assets/img/trainup_screenshot.png' | relative_url }}" alt="TrainUp screenshot" class="card-img">
      <div class="card-body">
        <h3>TrainUp — Traineeship Matching</h3>
        <p>Platform connecting students, professors, and companies; roles, requests, matching, and notifications.</p>
        <p class="tech">Spring Boot, Thymeleaf, MySQL, Bootstrap</p>
        <div class="card-actions">
          <a class="btn small" href="https://github.com/YOUR_GITHUB_USERNAME/trainup" target="_blank">Repo</a>
        </div>
      </div>
    </article>

    <article class="card">
      <img src="{{ '/assets/img/socialbookstore.png' | relative_url }}" alt="SocialBookstore screenshot" class="card-img">
      <div class="card-body">
        <h3>SocialBookstore — Book Exchange & Ratings</h3>
        <p>Credit/points system, ratings, search & profiles; built for student communities.</p>
        <p class="tech">Java, MySQL, HTML/CSS/Bootstrap</p>
        <div class="card-actions">
          <a class="btn small" href="https://github.com/YOUR_GITHUB_USERNAME/socialbookstore" target="_blank">Repo</a>
        </div>
      </div>
    </article>
  </div>
</section>

<!-- About -->
<section class="section">
  <h2>About</h2>
  <p>
    I’m passionate about turning research into deployable systems. My diploma thesis focused on intelligent robot navigation in dynamic pedestrian scenarios,
    combining LiDAR & vision perception with decision-making algorithms. I also build full-stack apps and ML/CV pipelines.
  </p>
</section>

<!-- Skills -->
<section class="section">
  <h2>Skills</h2>
  <ul class="skills">
    <li><strong>Languages:</strong> Python, C/C++, Java, SQL</li>
    <li><strong>Frameworks:</strong> ROS, Spring Boot, OpenCV, PyTorch/TensorFlow</li>
    <li><strong>Tools:</strong> Git/GitHub, Docker, Gazebo, Linux/Ubuntu, LaTeX</li>
    <li><strong>Domains:</strong> Robotics, ML/CV, Full-Stack Web, Databases</li>
  </ul>
</section>

<!-- Footer -->
<footer class="footer">
  <span>© {{ site.time | date: '%Y' }} Konstantinos Christopoulos</span>
</footer>
