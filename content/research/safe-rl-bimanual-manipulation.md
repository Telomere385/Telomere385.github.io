---
title: "Safe RL for Bimanual Robotic Manipulation"
date: 2026-01-01
description: "Constrained reinforcement learning for a dual-arm KUKA iiwa manipulation task."
tags: ["safe-rl", "robotics", "bimanual-manipulation"]
showToc: true
---

## Overview

This is my ongoing research project, supervised by **Davide Tateo**, on safe reinforcement
learning for bimanual robotic manipulation. The setup uses two KUKA iiwa arms simulated in
**NVIDIA Isaac Sim**, with the goal of learning coordinated manipulation policies that respect
safety constraints throughout training and deployment.

## Approach

- **Algorithm**: Lagrangian Soft Actor-Critic (SAC), with adaptive Lagrange multipliers to
  balance task reward against constraint violation cost.
- **Framework**: Constrained Markov Decision Process (CMDP), where safety requirements are
  encoded as cost signals rather than hard-coded rules.
- **Simulation**: Dual KUKA iiwa arms in NVIDIA Isaac Sim, enabling parallelized training and
  realistic contact dynamics for bimanual coordination.

## Status

This project is currently in progress. More details, results, and eventual publications will
be added here as the work develops.

## Related Work

This project builds on methodology developed in an earlier course project — see
[Safe RL for Peg-in-a-Hole via Lagrangian SAC](/research/peg-in-a-hole-lagrangian-sac/).
