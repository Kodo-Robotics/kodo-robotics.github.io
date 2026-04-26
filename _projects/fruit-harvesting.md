---
title: "Autonomous Fruit Harvesting System"
excerpt: "Perception-driven UR10 manipulation pipeline with task planning and collision-aware execution."
outcome: "A UR10 manipulation pipeline that plans, detects, and executes picks with collision awareness — no manual parameter tuning per fruit."
header:
    teaser: "/assets/images/projects/fruit-harvesting/hero.png"
    overlay_image: "/assets/images/projects/fruit-harvesting/hero.png"
    overlay_filter: 0.3
---

## Overview

A complete simulation pipeline for autonomous fruit harvesting using a UR10 manipulator in Gazebo.

The system integrates perception, motion planning, and task orchestration into a deterministic workflow.

---

## System Architecture

- UR10 robot model with custom orchard environment
- YOLO-based apple detection
- 3D pose estimation from RGB camera stream
- MoveIt 2 motion planning with collision avoidance
- State machine driven task planning
- Pick → place execution pipeline

---

## Engineering Focus

- Clean separation between perception and control layers
- Robust collision checking within cluttered tree environment
- Deterministic task sequencing
- Simulation-first validation for deployment readiness

---

## Outcome

A full-stack manipulation system demonstrating perception-to-action autonomy in a constrained agricultural scenario.

<video width="100%" autoplay loop muted playsinline>
  <source src="/assets/videos/projects/fruit-harvesting/demo.mp4" type="video/mp4">
</video>

<div class="cta-section">
  <h2>Building a perception-driven manipulation pipeline that needs to work without manual tuning per object?</h2>
  <p>Getting detection, pose estimation, motion planning, and task sequencing to work together reliably in a cluttered environment is harder than any single piece in isolation. This project was about making that pipeline deterministic — from camera feed to confident pick execution — without hand-tuning for each new scenario.</p>
  <p class="cta-sub">If you are building a manipulation system that needs to go from perception to reliable action in an unstructured environment, we can help.</p>
  <a href="https://forms.gle/LADwun8N6qUuXpwh7" class="btn-primary" target="_blank" rel="noopener">Tell us about your project</a>
  <p class="cta-secondary">Or email <a href="mailto:kodorobotics@gmail.com">kodorobotics@gmail.com</a></p>
</div>