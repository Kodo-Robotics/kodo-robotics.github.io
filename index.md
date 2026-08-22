---
layout: home
author_profile: false
title: "Kodo Robotics"
---

# Kodo Robotics

## Building software infrastructure and systems for robotics.

Kodo Robotics develops tools and systems that help engineers build, simulate, validate, and deploy autonomous robots. The work spans ROS 2 architecture, simulation environments, autonomy stacks, and developer tooling.

[Explore projects](/projects/) · [Read engineering notes](/blog/)

---

## Engineering Focus

### Robotics Software
Modular software architecture for robot behavior, sensing, planning, and hardware interfaces.

### ROS 2 Systems
Composable ROS 2 systems, from package boundaries and launch configuration to navigation and manipulation.

### Simulation & Validation
Simulation environments and repeatable validation loops for testing assumptions before and alongside hardware experiments.

### Navigation, Manipulation & Developer Tools
Autonomy pipelines and practical tooling for reproducible builds, debugging, and faster engineering iteration.

---

## Engineering Principles

- Simulation-first validation
- Explicit failure and recovery behavior
- Modular, testable software boundaries
- Developer-friendly workflows
- Open work, experiments, and technical writing

---

## Engineering Case Studies

{% for project in site.projects %}
### [{{ project.title }}]({{ project.url | relative_url }})
{% if project.status %}*{{ project.status }}*{% endif %}

{{ project.excerpt | strip_html }}

{% endfor %}
[See all projects](/projects/)

---

## Engineering Notes

{% for post in site.posts limit:3 %}
### [{{ post.title }}]({{ post.url | relative_url }})

{{ post.excerpt | strip_html }}

{% endfor %}
[All engineering notes](/blog/)

---

Kodo Robotics is an independent robotics engineering initiative by Sakshay Mahna, a Robotics Software Engineer working on robotics software, simulation, and developer tooling.

[GitHub](https://github.com/Kodo-Robotics) · [LinkedIn](https://linkedin.com/in/sakshaymahna) · [Robotics with Sakshay](https://www.youtube.com/@RoboticswithSakshay)
