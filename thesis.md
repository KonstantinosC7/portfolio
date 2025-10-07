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
    <p class="muted">Clearpath Jackal • ROS Noetic • LiDAR Perception • Social-Force-Aware Navigation</p>
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
      <p>VLP-16 LiDAR (+ optional camera)</p>
    </div>
    <div class="kv">
      <h4>Stack</h4>
      <p>ROS Noetic, Gazebo</p>
    </div>
    <div class="kv">
      <h4>Keywords</h4>
      <p>Pedestrian detection, social forces (<em>pedsim_ros</em>), local avoidance</p>
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
    <li><strong>Perception:</strong> LiDAR clustering and association</li>
    <li><strong>Crowd Model:</strong> <code>pedsim_ros</code> social forces to simulate human motion and constraints.</li>
    <li><strong>Planning:</strong> Social-force-aware local planner with custom robot avoidance behavior.</li>
    <li><strong>Evaluation:</strong> Scenarios with varying pedestrian densities and speeds in Gazebo.</li>
  </ul>
  <p class="p-tech"><strong>Tech:</strong> Python, C++, ROS, Gazebo, VLP-16</p>
</section>

<section class="section">
  <h2>Demo</h2>
  <div class="video-wrap">
      <video controls width="720" poster="{{ '/assets/img/Diploma/0deg_no_obs.mov' | relative_url }}">
        <source src="{{ 'assets/img/Diploma/0deg_no_obs.mov' | relative_url }}" type="video/mp4">
      </video>
  </div>
</section>

<section class="section">
  <h2>Gallery</h2>
  <div class="gallery">
    <figure class="figure">
      <img src="{{ '/assets/img/Diploma/jackal_lab.jpg' | relative_url }}" alt="Lab setup">
      <figcaption>Lab setup — Jackal with VLP-16 LiDAR.</figcaption>
    </figure>
    <figure class="figure">
      <img src="{{ '/assets/img/Diploma/jackal_sim.jpg' | relative_url }}" alt="Simulation world">
      <figcaption>Jackal in Simulation Gazebo</figcaption>
    </figure>
    <figure class="figure">
      <img src="{{ '/assets/img/Diploma/forces_in_map.png' | relative_url }}" alt="Trajectories">
      <figcaption>Robot & Pedestrians Positions with Potential Field Forces and Obstacles.</figcaption>
    </figure>
  </div>
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
