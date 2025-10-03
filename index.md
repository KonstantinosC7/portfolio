---
layout: default
title: "Home"
---

<!-- Custom CSS -->
<link rel="stylesheet" href="{{ 'assets/css/style.css' | relative_url }}">

<!-- Top Navigation -->
<nav class="topbar">
  <div class="topbar-inner">
    <a class="brand-name" href="{{ '/' | relative_url }}">Konstantinos Christopoulos</a>

  <ul class="toplinks">
      <!-- add class="active" on the link that corresponds to the current page -->
      <li><a href="{{ '/thesis'   | relative_url }}" class="">Diploma Thesis</a></li>
      <li><a href="{{ '/projects' | relative_url }}" class="">Projects</a></li>
      <li><a href="{{ '/contact'  | relative_url }}" class="">Contact</a></li>
  </ul>
  </div>
</nav>


<section class="section">
  <div class="about-wrap">

    <!-- Left profile card -->
    <aside class="profile-card">
      <img src="{{ '/assets/img/profile.jpg' | relative_url }}" alt="Profile photo" class="avatar lg">
      <h3 class="name">Konstantinos Christopoulos</h3>
      <p class="role">Computer Science & Engineering</p>

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
        decision-making algorithms. I also build full-stack apps using Spring Boot.
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
            <li><strong>MSc, Computer Science & Engineering</strong><br>University of Ioannina</li>
            <li><strong>Thesis:</strong> Robot Navigation in Presence of People</li>
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
