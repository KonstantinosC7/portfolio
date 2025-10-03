---
layout: default
title: "Home"
---

<!-- Custom CSS -->
<link rel="stylesheet" href="{{ 'assets/css/style.css' | relative_url }}">

<!-- Top Navigation -->
<nav class="navbar">
  <div class="links">
    <a href="{{ '/projects' | relative_url }}">Projects</a>
    <a href="{{ '/contact' | relative_url }}">Contact</a>
  </div>
</nav>

<!-- Hero 
<header class="hero">
  <img src="{{ '/assets/img/profile.jpg' | relative_url }}" alt="Profile photo" class="avatar">
  <h1>Konstantinos Christopoulos</h1>
  <p class="tagline">Computer Engineering & Informatics Graduate — building intelligent systems in <strong>Robotics</strong>, <strong>ML</strong>, and <strong>Full-Stack</strong>.</p>
  <div class="cta">
    <a class="btn primary" href="{{ '/assets/CV_Konstantinos_Christopoulos.pdf' | relative_url }}" target="_blank">Download CV</a>
    <a class="btn" href="https://github.com/KonstantinosC7" target="_blank">GitHub</a>
    <a class="btn" href="https://www.linkedin.com/in/konstantinos-christopoulos-9365b3256" target="_blank">LinkedIn</a>
    <a class="btn ghost" href="mailto:christopoulosk218@gmail.com">Email me</a>
  </div>

  <div class="badges">
    <img alt="Python" src="https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=white">
    <img alt="ROS" src="https://img.shields.io/badge/ROS-22314E?logo=ros&logoColor=white">
    <img alt="Spring Boot" src="https://img.shields.io/badge/Spring%20Boot-6DB33F?logo=springboot&logoColor=white">
    <img alt="Git" src="https://img.shields.io/badge/Git-F05032?logo=git&logoColor=white">
  </div>
</header>-->


<!-- About -->
<section class="section">
  <h2>About</h2>
  <p>
    I’m passionate about turning research into deployable systems. My diploma thesis focused on intelligent robot navigation in dynamic pedestrian scenarios,
    combining LiDAR perception with decision-making algorithms. I also build full-stack apps.
  </p>
</section>

<section class="section">
  <div class="about-wrap">

    <!-- Left profile card -->
    <aside class="profile-card">
      <img src="{{ '/assets/img/profile.jpg' | relative_url }}" alt="Profile photo" class="avatar lg">
      <h3 class="name">Konstantinos Christopoulos</h3>
      <p class="role">Computer Engineering & Informatics</p>

      <div class="icon-row">
        <a href="mailto:christopoulosk218@gmail.com" title="Email">✉️</a>
        <a href="https://github.com/KonstantinosC7" target="_blank" title="GitHub">🐙</a>
        <a href="https://www.linkedin.com/in/konstantinos-christopoulos-9365b3256" target="_blank" title="LinkedIn">in</a>
      </div>
    </aside>

    <!-- Right content -->
    <main class="about-panel">
      <h2>About Me</h2>
      <p>
        I’m passionate about turning research into deployable systems. My diploma thesis focused on
        intelligent robot navigation in dynamic pedestrian scenarios, combining LiDAR perception with
        decision-making algorithms. I also build full-stack apps.
      </p>
      <a class="btn primary" href="{{ '/assets/CV_Konstantinos_Christopoulos.pdf' | relative_url }}" target="_blank">Download CV</a>

      <div class="cols">
        <section>
          <h3>Skills</h3>
          <ul class="list-dot">
            <li><strong>Languages:</strong> Python, C/C++, Java, SQL</li>
            <li><strong>Frameworks:</strong> ROS, Spring Boot, PyTorch/TensorFlow</li>
            <li><strong>Tools:</strong> Git/GitHub, Gazebo, Linux/Ubuntu, LaTeX</li>
            <li><strong>Domains:</strong> Robotics, ML, Full-Stack Web, Databases</li>
          </ul>
        </section>

        <section>
          <h3>Education</h3>
          <ul class="list-dot">
            <li><strong>BSc, Computer Engineering & Informatics</strong><br>University of Ioannina</li>
            <li><strong>Thesis:</strong> Robot Navigation in Crowded Environments</li>
          </ul>
        </section>
      </div>
    </main>

  </div>
</section>

<!-- Footer -->
<footer class="footer">
  <span>© {{ site.time | date: '%Y' }} Konstantinos Christopoulos</span>
</footer>
