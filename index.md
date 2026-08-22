---
layout: splash
author_profile: false
title: "Kodo Robotics"
excerpt: "Building software infrastructure and systems for robotics — ROS 2 architecture, simulation environments, autonomy stacks, and developer tooling."
header:
  overlay_color: "linear-gradient(160deg, #00adb5 0%, #252a34 65%)"
  actions:
    - label: "Explore Projects"
      url: "/projects/"
    - label: "Read Engineering Notes"
      url: "/blog/"
feature_row:
  - title: "Robotics Software"
    excerpt: "Modular software architecture for robot behavior, sensing, planning, and hardware interfaces."
  - title: "ROS 2 Systems"
    excerpt: "Composable ROS 2 systems, from package boundaries and launch configuration to navigation and manipulation."
  - title: "Simulation & Validation"
    excerpt: "Simulation environments and repeatable validation loops for testing assumptions before and alongside hardware experiments."
  - title: "Navigation, Manipulation & Developer Tools"
    excerpt: "Autonomy pipelines and practical tooling for reproducible builds, debugging, and faster engineering iteration."
---

## Engineering Focus

{% include feature_row %}

## Engineering Principles

- Simulation-first validation
- Explicit failure and recovery behavior
- Modular, testable software boundaries
- Developer-friendly workflows
- Open work, experiments, and technical writing

## Engineering Case Studies

<div class="entries-horizontal">
  {% for post in site.projects %}
    {% include archive-single.html type="horizontal" %}
  {% endfor %}
</div>

[See all projects](/projects/){: .btn .btn--light-outline .section-btn}

## Engineering Notes

<div class="entries-list">
  {% for post in site.posts limit:3 %}
    {% include archive-single.html type="list" %}
  {% endfor %}
</div>

[All engineering notes](/blog/){: .btn .btn--light-outline .section-btn}

---

Kodo Robotics is an independent robotics engineering initiative by Sakshay Mahna, a Robotics Software Engineer working on robotics software, simulation, and developer tooling.

[GitHub](https://github.com/Kodo-Robotics) · [LinkedIn](https://linkedin.com/in/sakshaymahna) · [Robotics with Sakshay](https://www.youtube.com/@RoboticswithSakshay)
