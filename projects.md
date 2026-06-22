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
        <h3>TrainUp — Traineeship Matching</h3>
      The aim of this project is to create an application that will help the University's Internship Committee monitor and manage both available and already assigned internship positions.   The application will mainly involve students, companies advertising positions, professors acting as supervisors, and the Committee overseeing the entire process.
        <ul class="p-bullets">
          <li>Committee workflow: roles, matching flow, notifications.</li>
          <li>Track available & assigned internship positions.</li>
        </ul>
        <p class="p-tech">Spring Boot, Thymeleaf, MySQL, HTML/CSS/Bootstrap</p>
        <div class="p-actions">
          <a class="btn small" href="https://github.com/KonstantinosC7/TrainUp" target="_blank">Repo</a>
          <a class="btn small ghost" href="https://github.com/KonstantinosC7/TrainUp/blob/main/reports/Project-description-v1.0.pdf" target="_blank">Report (PDF)</a>
        </div>
      </div>
    </article>

<!-- Diploma Projects Management App (Spring Boot) -->
<article class="p-card">
  <img class="p-thumb" src="{{ '/assets/img/ThesisLink/ThesisLink.png' | relative_url }}" alt="Diploma Projects Management App">
  <div class="p-body">
    <h3>Diploma Projects Management</h3>
    The goal of this project is to develop a web application that allows students to browse available thesis topics from various professors and apply for the thesis topics that interest them. The application also allows professors to assign thesis topics to students, supervise the thesis work assigned to them, and evaluate the results.
    <ul class="p-bullets">
      <li>Auth (login/register) with role-based views; CRUD for profiles, subjects, applications, theses; UML-driven layered design (DAO/Service/Controller).</li>
    </ul>
    <p class="p-tech">Spring Boot (MVC + Security), Thymeleaf, MySQL, JPA, UML, Maven</p>
    <div class="p-actions">
      <a class="btn small" href="https://github.com/KonstantinosC7/Thesis-Link" target="_blank">Repo</a>
      <a class="btn small ghost" href="{{ '/assets/reports/SprintReport_v1.pdf' | relative_url }}" target="_blank">Sprint Report (PDF)</a>
    </div>
  </div>
</article>

<!-- SpecFlow (Spring Boot) -->
<article class="p-card">
  <img class="p-thumb" src="{{ '/assets/img/SpecFlow/logo.png' | relative_url }}" alt="SpecFlow">
  <div class="p-body">
    <h3>SpecFlow</h3>
    This project develops a web-based Requirements Specification and Analysis application that supports collaborative software requirements definition and object-oriented analysis. Users can create structured Use Cases, generate CRC cards, link requirements to system components, and automatically export diagram scripts for tools such as PlantUML and Nomnoml. The platform bridges requirements gathering and software design in a secure and user-friendly environment. 
    <ul class="p-bullets">
      <li>Auth (login/register) with role-based views; CRUD for profiles, Projects, Use Caes, CRC Cards; UML-driven layered design (DAO/Service/Controller); Script for generating Diagrams</li>
    </ul>
    <p class="p-tech">Spring Boot (MVC + Security), Thymeleaf, MySQL, JPA, UML, Maven</p>
    <div class="p-actions">
      <a class="btn small" href="https://github.com/KonstantinosC7/SpecFlow" target="_blank">Repo</a>
      <a class="btn small ghost" href="{{ '/assets/reports/SprintReport_v1_SpecFlow.pdf' | relative_url }}" target="_blank">Sprint Report (PDF)</a>
    </div>
  </div>
</article>
    
<!-- Information Retrieval (Songs Search) -->
  <article class="p-card">
    <img class="p-thumb" src="{{ '/assets/img/Informationretrieval/Information-Retrieval.jpg' | relative_url }}" alt="Information Retrieval UI (songs search)">
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
    </div>
  </div>
</article>

<footer class="footer">
  <span>© {{ site.time | date: '%Y' }} Konstantinos Christopoulos</span>
</footer>
