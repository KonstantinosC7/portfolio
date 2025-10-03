---
layout: default
title: "Projects"
---

<link rel="stylesheet" href="{{ '/assets/css/style.css' | relative_url }}">

{% include topnav.html %}

<section class="section">
  <h1>Projects</h1>

  <div class="project-list">

    <!-- Robot Navigation -->
    <article class="p-card">
      <img class="p-thumb" src="{{ '/assets/img/Diploma/jackal_lab.jpg' | relative_url }}" alt="Robot Navigation">
      <div class="p-body">
        <h3>Robot Navigation in Presence of People</h3>
        Navi
        <ul class="p-bullets">
          <li>Navigation stack for Clearpath <strong>Jackal</strong> (ROS Noetic).</li>
          <li>LiDAR pedestrian detection + social-force-aware avoidance.</li>
          <li>Custom perception & planning modules; evaluated in realistic sims.</li>
        </ul>
        <p class="p-tech">Python, C++, ROS, Gazebo, VLP-16</p>
        <div class="p-actions">
          <a class="btn small" href="https://github.com/YOUR_GITHUB/robot-navigation" target="_blank">Repo</a>
          <a class="btn small" href="https://YOUR_DEMO_LINK" target="_blank">Demo</a>
          <a class="btn small ghost" href="{{ '/assets/reports/Robot_Navigation_Report.pdf' | relative_url }}" target="_blank">Report (PDF)</a>
        </div>
      </div>
    </article>

    <!-- TrainUp -->
    <article class="p-card">
      <img class="p-thumb" src="{{ '/assets/img/TrainUp/TrainUp.jpg' | relative_url }}" alt="TrainUp">
      <div class="p-body">
      The aim of this project is to create an application that will help the University's Internship Committee monitor and manage both available and already assigned internship positions.   The application will mainly involve students, companies advertising positions, professors acting as supervisors, and the Committee overseeing the entire process.
        <h3>TrainUp — Traineeship Matching</h3>
        <ul class="p-bullets">
          <li>Committee workflow: roles, matching flow, notifications.</li>
          <li>Track available & assigned internship positions.</li>
        </ul>
        <p class="p-tech">Spring Boot, Thymeleaf, MySQL, HTML/CSS/Bootstrap</p>
        <div class="p-actions">
          <a class="btn small" href="https://github.com/YOUR_GITHUB/trainup" target="_blank">Repo</a>
          <a class="btn small ghost" href="{{ '/assets/img/trainup_gallery/' | relative_url }}" target="_blank">Screens</a>
        </div>
      </div>
    </article>

<footer class="footer">
  <span>© {{ site.time | date: '%Y' }} Konstantinos Christopoulos</span>
</footer>
