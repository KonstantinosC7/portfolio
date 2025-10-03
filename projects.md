---
layout: default
title: "Projects"
---

<link rel="stylesheet" href="{{ '/assets/css/style.css' | relative_url }}">

<nav class="navbar">
  <div class="nav-inner">
    <a class="brand" href="{{ '/' | relative_url }}">KC</a>
    <div class="links">
      <a href="{{ '/' | relative_url }}">Home</a>
      <a class="active" href="{{ '/projects' | relative_url }}">Projects</a>
      <a href="{{ '/contact' | relative_url }}">Contact</a>
    </div>
  </div>
</nav>

<section class="section">
  <h1>Projects</h1>
  <p class="muted">Compact view with thumbnails, brief description, tech, and quick actions.</p>

  <table class="proj-table">
    <thead>
      <tr>
        <th>Project</th>
        <th>Description</th>
        <th>Tech</th>
        <th>Links</th>
      </tr>
    </thead>

    <tbody>
      <!-- Robot Navigation -->
      <tr>
        <td class="proj-title">
          <img class="thumb" src="{{ '/assets/img/jackal_demo.jpg' | relative_url }}" alt="Robot Navigation">
          <div>
            <strong>Robot Navigation in Presence of People</strong><br>
            <span class="muted">Clearpath Jackal • ROS Noetic</span>
          </div>
        </td>
        <td>
          Navigation stack with LiDAR pedestrian detection and social-force-aware avoidance;
          tested in realistic sim worlds with custom modules for perception & planning.
        </td>
        <td>
          Python, C++, ROS, Gazebo, VLP-16 LiDAR, OpenCV/YOLO
        </td>
        <td class="proj-actions">
          <a class="btn small"  href="https://github.com/YOUR_GITHUB/robot-navigation" target="_blank">Repo</a>
          <a class="btn small"  href="https://YOUR_DEMO_LINK" target="_blank">Demo</a>
          <a class="btn small ghost" href="{{ '/assets/reports/Robot_Navigation_Report.pdf' | relative_url }}" target="_blank">Report (PDF)</a>
        </td>
      </tr>

      <!-- TrainUp -->
      <tr>
        <td class="proj-title">
          <img class="thumb" src="{{ '/assets/img/trainup_screenshot.png' | relative_url }}" alt="TrainUp">
          <div>
            <strong>TrainUp — Traineeship Matching</strong><br>
            <span class="muted">Internship workflow app</span>
          </div>
        </td>
        <td>
          Web platform that helps the University’s Internship Committee manage available and assigned positions,
          with roles, matching flow, and notifications.
        </td>
        <td>
          Spring Boot, Thymeleaf, MySQL, Bootstrap
        </td>
        <td class="proj-actions">
          <a class="btn small" href="https://github.com/YOUR_GITHUB/trainup" target="_blank">Repo</a>
          <a class="btn small ghost" href="{{ '/assets/img/trainup_gallery/' | relative_url }}" target="_blank">Screens</a>
        </td>
      </tr>

      <!-- SocialBookstore -->
      <tr>
        <td class="proj-title">
          <img class="thumb" src="{{ '/assets/img/socialbookstore.png' | relative_url }}" alt="SocialBookstore">
          <div>
            <strong>SocialBookstore — Book Exchange & Ratings</strong><br>
            <span class="muted">Student communities</span>
          </div>
        </td>
        <td>
          Credit/points system, ratings & reviews, search, and profiles to enable book exchange inside student groups.
        </td>
        <td>
          Java, MySQL, HTML/CSS/Bootstrap
        </td>
        <td class="proj-actions">
          <a class="btn small" href="https://github.com/YOUR_GITHUB/socialbookstore" target="_blank">Repo</a>
        </td>
      </tr>
    </tbody>
  </table>
</section>

<footer class="footer">
  <span>© {{ site.time | date: '%Y' }} Konstantinos Christopoulos</span>
</footer>
