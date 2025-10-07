---
layout: default
title: "Projects"
nav_active: projects
---

<link rel="stylesheet" href="{{ '/assets/css/style.css' | relative_url }}">

{% include topnav.html %}

<section class="section">
  <h1>Projects</h1>

  <div class="project-list">
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
        </div>
      </div>
    </article>

<footer class="footer">
  <span>© {{ site.time | date: '%Y' }} Konstantinos Christopoulos</span>
</footer>
