---
layout: default
title: "Home"
nav_active: home
---

<!-- Custom CSS -->
<link rel="stylesheet" href="{{ 'assets/css/style.css' | relative_url }}">

{% include topnav.html %}


<section class="section">
  <div class="about-wrap">

    <!-- Left profile card -->
    <aside class="profile-card">
      <img src="{{ '/assets/img/profile.jpg' | relative_url }}" alt="Profile photo" class="avatar lg">
      <h3 class="name">Konstantinos Christopoulos</h3>
      <p class="role">Computer Science & Engineering</p>

      <div class="icon-row">
        <a href="mailto:christopoulosk218@gmail.com" title="Email">✉️
        <a href="mailto:christopoulosk218@gmail.com" title="Email" class="gmail">
    <!-- Gmail-style envelope (inline SVG) -->
  <svg width="20" height="20" viewBox="0 0 24 24" aria-hidden="true">
    <!-- Red envelope background -->
    <path fill="#EA4335" d="M3 6.75C3 5.78 3.78 5 4.75 5h14.5C20.22 5 21 5.78 21 6.75v10.5A1.75 1.75 0 0 1 19.25 19H4.75A1.75 1.75 0 0 1 3 17.25V6.75z"/>
    <!-- White 'M' -->
    <path fill="#FFFFFF" d="M19 8.5v8h-2v-6.2l-5 3.7-5-3.7V16.5H5v-8l7 5.2 7-5.2z"/>
  </svg>
</a>
</a>
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
