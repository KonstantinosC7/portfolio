---
layout: default
title: "Diploma Thesis"
nav_active: thesis
---

<link rel="stylesheet" href="{{ '/assets/css/style.css' | relative_url }}">

{% include topnav.html %}

<section class="section thesis-hero">
  <div class="thesis-title">
    <h1>Robot Navigation in Presence of People</h1>
    <p class="muted">Clearpath Jackal • ROS Noetic • LiDAR Perception • Social-Force-Model • Potential Fields</p>
    <div class="thesis-actions">
      <a class="btn primary" href="{{ 'assets/reports/Diploma_Thesis_Robotics.pdf' | relative_url }}" target="_blank">Download Report (PDF)</a>
      <a class="btn" href="https://github.com/YOUR_GITHUB/robot-navigation" target="_blank">Repository</a>
      <a class="btn ghost" href="{{ '/assets/reports/Robot_Navigation_Presentation.pdf' | relative_url }}" target="_blank">Slides</a>
    </div>
  </div>

  <div class="thesis-hero-media">
    <img src="{{ '/assets/img/Diploma/Robot-Navigation.png' | relative_url }}" alt="Jackal setup" class="hero-shot">
  </div>
</section>

<section class="section">
  <div class="kv-cards">
    <div class="kv">
      <h4>Robot</h4>
      <p>Clearpath <strong>Jackal</strong></p>
    </div>
    <div class="kv">
      <h4>Sensors</h4>
      <p>VLP-16 LiDAR</p>
    </div>
    <div class="kv">
      <h4>Stack</h4>
      <p>ROS Noetic, Gazebo, RViz</p>
    </div>
  </div>
</section>

<section class="section">
  <h2>Abstract</h2>
  <p>
   In this thesis, we present a novel multi-step pedestrian avoidance framework for mobile robots
  navigating dynamic environments. The proposed system integrates <strong>LiDAR-based pedestrian
  tracking, dynamic obstacle detection, and potential field navigation</strong> to ensure safe and efficient
  robot movement in human spaces. We implement on the Jackal robot, integrating advanced
  hardware components such as the <strong>Velodyne VLP-16 LiDAR</strong> to collect rich 3D point cloud
  data. The avoidance methodology employs multi-step filtering to distinguish static and dynamic
  obstacles, <strong>dynamic point clustering via DBSCAN, and Kalman filters</strong> for robust pedestrian
  tracking and prediction pedestrian trajectories. As far as the pedestrian movement, we use the
  <strong>Social Force Model (SFM)</strong>, combining attractive and repulsive forces. A <strong>potential field</strong> approach,
  guides the robot toward a safe destination, while maintaining real-time adaptability to changing
  conditions.
  </p>
</section>

<section class="section">
  <h2>Method</h2>
  <ul class="list-dot">
    <li><strong>Pedestrians:</strong> <code>pedsim_ros</code> social forces to simulate human motion and constraints.</li>
    <li><strong>Detection Pedestrian:</strong> LiDAR clustering (DBSCAN) and association.</li>
    <li><strong>Tracking Pedestrian:</strong> Kalman filters for predicting pedestrian movement.</li>
    <li><strong>Pedestrian Avoidance:</strong> determination of the best free point for the robot to move.</li>
    <li><strong>Robot Movement:</strong> Potential Fields for moving the robot to the selected point in the map.</li>
  </ul>
  <p class="p-tech"><strong>Tech:</strong> Python, C++, ROS, Gazebo, VLP-16</p>
</section>


<!-- Video --> 
<section class="section">
  <h2>Video</h2>
  <div class="video-wrap">
      <video controls width="720" poster="{{ '/assets/img/Diploma/0deg_no_obs.mov' | relative_url }}">
        <source src="{{ 'assets/img/Diploma/0deg_no_obs.mov' | relative_url }}" type="video/mp4">
      </video>
  </div>
</section>


<!-- Gallery --> 
<section class="section">
  <h2>Gallery</h2>

  <div class="gallery-grid">
    <!-- Each tile -->
    <figure class="g-item">
      <img src="{{ '/assets/img/Diploma/jackal_lab.jpg' | relative_url }}" alt="Lab setup — Jackal with VLP-16 LiDAR" data-caption="Lab setup — Jackal with VLP-16 LiDAR">
      <figcaption>Lab setup — Jackal with VLP-16 LiDAR.</figcaption>
    </figure>
    <figure class="g-item">
      <img src="{{ '/assets/img/Diploma/jackal_sim.jpg' | relative_url }}" alt="Jackal in Simulation Gazebo" data-caption="Jackal in Simulation Gazebo">
      <figcaption>Jackal in Simulation Gazebo</figcaption>
    </figure>
    <figure class="g-item">
      <img src="{{ '/assets/img/Diploma/forces_in_map.png' | relative_url }}" alt="Robot & Pedestrians with forces/obstacles" data-caption="Robot & Pedestrians — forces and obstacles">
      <figcaption>Robot & Pedestrians Positions with Potential Field Forces and Obstacles.</figcaption>
    </figure>
  </div>

  <!-- Lightbox viewer -->
  <div class="lightbox" id="lightbox" aria-hidden="true">
    <button class="lb-close" aria-label="Close">×</button>
    <button class="lb-prev" aria-label="Previous">‹</button>
    <img class="lb-img" alt="">
    <div class="lb-caption"></div>
    <button class="lb-next" aria-label="Next">›</button>
  </div>

  <script>
    // Minimal vanilla JS lightbox
    (function(){
      const tiles = Array.from(document.querySelectorAll('.gallery-grid .g-item img'));
      const box = document.getElementById('lightbox');
      const img = box.querySelector('.lb-img');
      const cap = box.querySelector('.lb-caption');
      const closeBtn = box.querySelector('.lb-close');
      const prevBtn = box.querySelector('.lb-prev');
      const nextBtn = box.querySelector('.lb-next');
      let i = 0;

      function open(idx){
        i = idx;
        const el = tiles[i];
        img.src = el.src;
        img.alt = el.alt || '';
        cap.textContent = el.dataset.caption || el.alt || '';
        box.setAttribute('aria-hidden','false');
        document.body.style.overflow = 'hidden';
      }
      function close(){
        box.setAttribute('aria-hidden','true');
        document.body.style.overflow = '';
      }
      function prev(){ open( (i - 1 + tiles.length) % tiles.length ); }
      function next(){ open( (i + 1) % tiles.length ); }

      tiles.forEach((t, idx) => t.addEventListener('click', () => open(idx)));
      closeBtn.addEventListener('click', close);
      box.addEventListener('click', (e)=>{ if(e.target===box) close(); });
      prevBtn.addEventListener('click', prev);
      nextBtn.addEventListener('click', next);
      document.addEventListener('keydown', (e)=>{
        if(box.getAttribute('aria-hidden')==='true') return;
        if(e.key==='Escape') close();
        if(e.key==='ArrowLeft') prev();
        if(e.key==='ArrowRight') next();
      });

      // touch swipe
      let startX=0;
      box.addEventListener('touchstart',(e)=> startX = e.touches[0].clientX, {passive:true});
      box.addEventListener('touchend',(e)=>{
        const dx = e.changedTouches[0].clientX - startX;
        if(Math.abs(dx) > 40) (dx>0? prev: next)();
      });
    })();
  </script>
</section>


<section class="section">
  <h2>Results &amp; Notes</h2>
  <ul class="list-dot">
    <li>Real-time pedestrian detection and avoidance. Works well in dynamic environments.</li>
    <li>Modular ROS design, easy extendable.</li>
    <li>Integration of additional sensing modalities, such as 3D cameras.</li>
  </ul>
</section>

<footer class="footer">
  <span>© {{ site.time | date: '%Y' }} Konstantinos Christopoulos</span>
</footer>
