---
layout: default
title: "Contact"
---

<link rel="stylesheet" href="{{ '/assets/css/style.css' | relative_url }}">

<nav class="navbar">
  <div class="links">
    <a href="{{ '/' | relative_url }}">Home</a>
    <a href="{{ '/projects' | relative_url }}">Projects</a>
  </div>
</nav>

<section class="section">
  <h1>Contact</h1>
  <p class="muted">Quick facts in one place.</p>

  <table class="kv-table">
    <tr>
      <th>Email</th>
      <td><a href="mailto:christopoulosK218@gmail.com">christopoulosK218@gmail.com</a></td>
    </tr>
    <tr>
      <th>Location</th>
      <td>📍 Athens, Greece</td>
    </tr>
    <tr>
      <th>CV</th>
      <td><a href="{{ '/assets/CV_Konstantinos_Christopoulos.pdf' | relative_url }}" target="_blank">Download my CV (PDF)</a></td>
    </tr>
    <tr>
      <th>LinkedIn</th>
      <td><a href="https://www.linkedin.com/in/konstantinos-christopoulos" target="_blank">linkedin.com/in/konstantinos-christopoulos</a></td>
    </tr>
    <tr>
      <th>GitHub</th>
      <td><a href="https://github.com/KonstantinosC7" target="_blank">github.com/KonstantinosC7</a></td>
    </tr>
  </table>
</section>

<footer class="footer">
  <span>© {{ site.time | date: '%Y' }} Konstantinos Christopoulos</span>
</footer>



  <!-- (Optional) Formspree contact form — replace YOUR_FORMSPREE_ID
  <form action="https://formspree.io/f/YOUR_FORMSPREE_ID" method="POST" class="contact-form">
    <input type="text" name="name" placeholder="Your name" required>
    <input type="email" name="_replyto" placeholder="Your email" required>
    <textarea name="message" placeholder="Your message" rows="6" required></textarea>
    <button type="submit" class="btn primary">Send</button>
  </form>
  -->
