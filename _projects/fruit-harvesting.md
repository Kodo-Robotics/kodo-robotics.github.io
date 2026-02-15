---
title: "Autonomous Fruit Harvesting System"
excerpt: "Perception-driven UR10 manipulation pipeline with task planning and collision-aware execution."
header:
    teaser: "/assets/images/projects/fruit-harvesting/hero.png"
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