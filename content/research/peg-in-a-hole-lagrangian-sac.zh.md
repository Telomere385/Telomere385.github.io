---
title: "基于 Lagrangian SAC 的孔轴装配安全强化学习"
date: 2026-01-01
description: "EDAN70 课程项目：面向孔轴装配任务的安全强化学习。"
tags: ["safe-rl", "robotics", "course-project"]
showToc: true
---

## 项目概述

这是我在 EDAN70 课程中完成的项目，与合作者 **Miao Xu** 共同完成，由 **Davide Tateo** 指导。
项目使用安全强化学习方法解决孔轴装配（peg-in-a-hole）任务，最终整理为 IEEE 格式论文并配有展示报告。

## 方法

- **算法**：Lagrangian SAC，通过自适应拉格朗日乘子实现约束策略优化。
- **框架**：扩展了 [MushroomRL](https://github.com/MushroomRL/mushroom-rl) 的经验回放缓冲区以支持代价信号，
  从而支持约束马尔可夫决策过程（CMDP）框架下的训练。
- **课程设计**：在 Isaac Sim 中设计了三阶段几何课程学习方案，逐步提升任务难度，以稳定训练过程并提升最终策略表现。

## 实验结果

训练得到的策略成功完成了孔轴装配任务，并在整个训练过程中满足了安全约束，
证明了相较于直接在完整任务难度上训练，几何课程学习方案带来的优势。

## 论文 / 报告

- Ruining Wang, Miao Xu (2026). *Safe Reinforcement Learning for Peg-in-a-Hole using
  Lagrangian SAC*. 隆德大学课程项目。
