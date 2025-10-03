---
layout: default
title: "Contact"
---

<link rel="stylesheet" href="{{ '/assets/css/style.css' | relative_url }}">

<nav class="navbar">
  <div class="nav-inner">
    <a class="brand" href="{{ '/' | relative_url }}">KC</a>
    <div class="links">
      <a href="{{ '/' | relative_url }}">Home</a>
      <a href="{{ '/projects' | relative_url }}">Projects</a>
      <a class="active" href="{{ '/contact' | relative_url }}">Contact</a>
    </div>
  </div>
</nav>

<section class="section">
  <h1>Contact</h1>

- 📧 Email: <a href="mailto:christopoulosk218@gmail.com">christopoulosk218@gmail.com</a>
- - 📍 Athens, Greece
- ⬇️ [Download my CV]()
- 🔗 LinkedIn: <a href="https://www.linkedin.com/in/konstantinos-christopoulos-9365b3256" target="_blank">Linkedin</a>  
- 💻 GitHub: <a href="https://www.linkedin.com/in/konstantinos-christopoulos-9365b3256" target="_blank">GitHub</a>

  <!-- (Optional) Formspree contact form — replace YOUR_FORMSPREE_ID
  <form action="https://formspree.io/f/YOUR_FORMSPREE_ID" method="POST" class="contact-form">
    <input type="text" name="name" placeholder="Your name" required>
    <input type="email" name="_replyto" placeholder="Your email" required>
    <textarea name="message" placeholder="Your message" rows="6" required></textarea>
    <button type="submit" class="btn primary">Send</button>
  </form>
  -->
</section>

<footer class="footer">
  <span>© {{ site.time | date: '%Y' }} Konstantinos Christopoulos</span>
</footer>
