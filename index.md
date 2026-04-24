---
layout: single
author_profile: false
classes: wide
---

<section class="hero-section">
  <h1 class="hero-headline">Your ROS&nbsp;2 robot, production-ready.</h1>
  <p class="hero-subheadline">Most robotics teams get stuck between prototype and reliable deployment. We specialise in the gap — using simulation-first development so your system is validated before it ever touches hardware.</p>
  <div class="hero-ctas">
    <a href="#book" class="btn-primary">Book a free 30-min call</a>
    <a href="/projects/" class="btn-secondary">See our work →</a>
  </div>
</section>

<div class="credibility-bar">
  <p>4 production systems built · ROS 2 / Nav2 / MoveIt 2 · Isaac Sim · Gazebo · AgileX · UR10 · Jetson deployment</p>
</div>

<section class="services-section">
  <h2 class="section-header">What we do</h2>
  <div class="services-grid">
    <div class="service-card">
      <h3>Autonomous Navigation</h3>
      <p>Your robot finds its way reliably — in warehouses, outdoors, or complex environments. We build and tune the Nav2 stack that gets it there without constant intervention.</p>
    </div>
    <div class="service-card">
      <h3>Manipulation Software</h3>
      <p>Your robot arm picks, places, and executes tasks precisely. We integrate MoveIt 2, handle collision planning, and make sure it works in the real world, not just in demos.</p>
    </div>
    <div class="service-card">
      <h3>Simulation &amp; Validation</h3>
      <p>Your system is tested to failure before you spend a day on hardware. We build high-fidelity simulation environments in Isaac Sim, Gazebo, or Unreal so problems surface in software, not on the floor.</p>
    </div>
    <div class="service-card">
      <h3>Production Deployment</h3>
      <p>Your robot ships. Dockerized ROS 2 environments, CI/CD pipelines, and Jetson/NUC deployments that your team can maintain and scale.</p>
    </div>
  </div>
</section>

<section class="philosophy-section">
  <h2 class="section-header">How we work</h2>
  <div class="philosophy-grid">
    <div class="philosophy-item">
      <h4>Simulation-first</h4>
      <p>We validate in sim before touching hardware.</p>
    </div>
    <div class="philosophy-item">
      <h4>Deterministic</h4>
      <p>No surprises in production.</p>
    </div>
    <div class="philosophy-item">
      <h4>Clean architecture</h4>
      <p>Code your team can own and extend.</p>
    </div>
    <div class="philosophy-item">
      <h4>Reproducible builds</h4>
      <p>Same result every time, everywhere.</p>
    </div>
    <div class="philosophy-item">
      <h4>Systems thinking</h4>
      <p>We fix root causes, not symptoms.</p>
    </div>
  </div>
</section>

<section class="projects-section">
  <h2 class="section-header">Recent work</h2>
  <div class="homepage-projects-grid">
    {% for project in site.projects %}
    <div class="homepage-project-card">
      {% if project.header.teaser %}
      <a href="{{ project.url | relative_url }}">
        <img src="{{ project.header.teaser | relative_url }}" alt="{{ project.title }}" class="project-card-img">
      </a>
      {% endif %}
      <div class="project-card-body">
        {% if project.outcome %}
        <p class="project-outcome">{{ project.outcome }}</p>
        {% endif %}
        <h3><a href="{{ project.url | relative_url }}">{{ project.title }}</a></h3>
        <p class="project-excerpt">{{ project.excerpt | strip_html | truncate: 120 }}</p>
      </div>
    </div>
    {% endfor %}
  </div>
  <div class="see-all-link">
    <a href="/projects/">See all projects →</a>
  </div>
</section>

<section class="blog-section">
  <h2 class="section-header">Recent writing</h2>
  <div class="homepage-blog-list">
    {% for post in site.posts limit:3 %}
    <div class="homepage-blog-item">
      {% if post.audience_tag %}
      <span class="audience-tag">For: {{ post.audience_tag }}</span>
      {% endif %}
      <h3><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
      <p class="post-excerpt">{{ post.excerpt | strip_html | truncate: 140 }}</p>
    </div>
    {% endfor %}
  </div>
</section>

<section class="cta-section" id="book">
  <h2>Ready to move from prototype to production?</h2>
  <p>We work with teams building production robotic systems — startups, hardware companies, and R&amp;D labs. If that's you, book a technical scoping call below.</p>
  <p class="cta-sub">We'll look at where your system is stuck, whether we're a fit, and what the path to reliable deployment looks like.</p>
  <a href="https://calendly.com/kodorobotics/30min" class="btn-primary">Book a call</a>
  <p class="cta-secondary">Or email <a href="mailto:kodorobotics@gmail.com">kodorobotics@gmail.com</a></p>
</section>
