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
      <!-- Information Retrieval (Songs Search) -->
<article class="p-card">
  <img class="p-thumb" src="{{ '/assets/img/InformationRetrieval/ir_ui.png' | relative_url }}" alt="Information Retrieval UI (songs search)">
  <div class="p-body">
    <h3>Information Retrieval — Songs Search Engine</h3>
    <ul class="p-bullets">
      <li>Indexes song data from CSV with <strong>Apache Lucene</strong>; fast keyword search.</li>
      <li>Filters by <em>Artist</em>, <em>Song</em>, or <em>Lyrics</em> with optional <em>Alphabetical Grouping</em>.</li>
      <li>Web view with query history, ranked results, and full-lyrics page (next/prev).</li>
    </ul>
    <p class="p-tech">Java, Apache Lucene, CSV parsing, Web UI</p>
    <div class="p-actions">
      <a class="btn small" href="https://github.com/KonstantinosC7/InformationRetrieval" target="_blank">Repo</a>
      <!-- Option A: link to the PDF in GitHub -->
      <a class="btn small ghost" href="https://github.com/KonstantinosC7/InformationRetrieval/blob/main/Report_Information_Retrieval.pdf" target="_blank">Report (PDF)</a>
      <!-- Option B (recommended): copy the PDF into your site at /assets/reports/ then use: 
      <a class="btn small ghost" href="{{ '/assets/reports/Report_Information_Retrieval.pdf' | relative_url }}" target="_blank">Report (PDF)</a>
      -->
    </div>
  </div>
</article>

    </div>
    </article>

<footer class="footer">
  <span>© {{ site.time | date: '%Y' }} Konstantinos Christopoulos</span>
</footer>
