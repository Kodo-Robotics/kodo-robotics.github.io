---
layout: single
author_profile: false
classes: wide
---

<section class="hero-section">
  <h1 class="hero-headline">Building software infrastructure and systems for robotics.</h1>
  <p class="hero-subheadline">Kodo Robotics develops tools and systems that help engineers build, simulate, validate, and deploy autonomous robots. The work spans ROS 2 architecture, simulation environments, autonomy stacks, and developer tooling.</p>
  <div class="hero-ctas">
    <a href="/projects/" class="btn-primary">Explore projects</a>
    <a href="/blog/" class="btn-secondary">Read engineering notes →</a>
  </div>
</section>

<div class="credibility-bar">
  <p>ROS 2 · Nav2 · MoveIt 2 · Gazebo · Isaac Sim · robot simulation · hardware validation</p>
</div>

<section class="services-section">
  <h2 class="section-header">Engineering focus</h2>
  <div class="services-grid">
    <div class="service-card">
      <h3>Robotics Software</h3>
      <p>Modular software architecture for robot behavior, sensing, planning, and hardware interfaces that remains understandable as systems grow.</p>
    </div>
    <div class="service-card">
      <h3>ROS 2 Systems</h3>
      <p>Composable ROS 2 systems, from package boundaries and launch configuration to navigation, manipulation, and deployment workflows.</p>
    </div>
    <div class="service-card">
      <h3>Simulation &amp; Validation</h3>
      <p>Simulation environments and repeatable validation loops for testing assumptions before and alongside real-hardware experiments.</p>
    </div>
    <div class="service-card">
      <h3>Navigation &amp; Manipulation</h3>
      <p>Autonomy pipelines that connect perception, planning, controls, and task execution in constrained, changing environments.</p>
    </div>
    <div class="service-card">
      <h3>Developer Tools</h3>
      <p>Practical tooling for reproducible builds, experiment setup, debugging, and faster iteration across robotics software projects.</p>
    </div>
  </div>
</section>

<section class="philosophy-section">
  <h2 class="section-header">Engineering principles</h2>
  <div class="philosophy-grid">
    <div class="philosophy-item">
      <h4>Simulation-first</h4>
      <p>Use simulation to explore, test, and narrow uncertainty before hardware trials.</p>
    </div>
    <div class="philosophy-item">
      <h4>Reliable systems</h4>
      <p>Make failure modes visible and recovery behavior explicit.</p>
    </div>
    <div class="philosophy-item">
      <h4>Modular design</h4>
      <p>Keep interfaces clear so components can be tested and extended independently.</p>
    </div>
    <div class="philosophy-item">
      <h4>Developer experience</h4>
      <p>Build tools and workflows that reduce friction during iteration and debugging.</p>
    </div>
    <div class="philosophy-item">
      <h4>Open work</h4>
      <p>Share useful tools, lessons, and experiments with the robotics community.</p>
    </div>
  </div>
</section>

<section class="projects-section">
  <h2 class="section-header">Engineering case studies</h2>
  <div class="homepage-projects-grid">
    {% for project in site.projects %}
    <div class="homepage-project-card">
      {% if project.header.teaser %}
      <a href="{{ project.url | relative_url }}">
        <img src="{{ project.header.teaser | relative_url }}" alt="{{ project.title }}" class="project-card-img">
      </a>
      {% endif %}
      <div class="project-card-body">
        {% if project.status %}
        <span class="project-status">{{ project.status }}</span>
        {% endif %}
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
  <h2 class="section-header">Engineering notes</h2>
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

<section class="cta-section">
  <h2>Built by Sakshay Mahna</h2>
  <p>Kodo Robotics is an independent robotics engineering initiative by Sakshay Mahna, a Robotics Software Engineer working on robotics software, simulation, and developer tooling.</p>
  <a href="https://github.com/Kodo-Robotics" class="btn-primary" target="_blank" rel="noopener">Follow on GitHub</a>
  <p class="cta-secondary"><a href="https://linkedin.com/in/sakshaymahna" target="_blank" rel="noopener">LinkedIn</a> · <a href="https://www.youtube.com/@RoboticswithSakshay" target="_blank" rel="noopener">Robotics with Sakshay on YouTube</a></p>
</section>
