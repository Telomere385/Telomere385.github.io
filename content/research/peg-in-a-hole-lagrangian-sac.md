---
title: "Safe RL for Peg-in-a-Hole via Lagrangian SAC"
date: 2026-01-01
description: "EDAN70 course project: safe reinforcement learning for a peg-in-a-hole assembly task."
tags: ["safe-rl", "robotics", "course-project"]
showToc: true
---

## Overview

This was my EDAN70 course project, completed with partner **Miao Xu** under the supervision of
**Davide Tateo**. The project tackled a peg-in-a-hole assembly task using safe reinforcement
learning, and was written up as an IEEE-format paper with an accompanying presentation.

## Methods

- **Algorithm**: Lagrangian SAC with adaptive Lagrange multipliers for constrained policy
  optimization.
- **Framework**: Extended [MushroomRL](https://github.com/MushroomRL/mushroom-rl)'s replay
  buffer to support cost signals, enabling training under a Constrained Markov Decision
  Process (CMDP) formulation.
- **Curriculum**: Designed a three-stage geometric curriculum in Isaac Sim, progressively
  increasing task difficulty to stabilize training and improve final policy performance.

## Results

The trained policy successfully learned to complete the peg-in-a-hole task while respecting
safety constraints throughout training, demonstrating the benefit of the geometric curriculum
over training on the full task difficulty from the start.

## Publications

- Ruining Wang, Miao Xu (2026). *Safe Reinforcement Learning for Peg-in-a-Hole using
  Lagrangian SAC*. Course project, Lund University.
