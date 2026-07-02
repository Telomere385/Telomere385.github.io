---
title: "面向双臂机器人操作的安全强化学习"
date: 2026-01-01
description: "面向双臂 KUKA iiwa 操作任务的约束强化学习研究。"
tags: ["safe-rl", "robotics", "bimanual-manipulation"]
showToc: true
---

## 项目概述

这是我正在进行中的研究项目，由 **Davide Tateo** 指导，聚焦于双臂机器人操作场景下的安全强化学习。
实验平台基于 **NVIDIA Isaac Sim** 中仿真的两台 KUKA iiwa 机械臂，目标是在训练与部署全过程中，
学习既能完成协同操作任务、又能满足安全约束的策略。

## 方法

- **算法**：Lagrangian Soft Actor-Critic（SAC），通过自适应拉格朗日乘子在任务奖励与约束违反代价之间取得平衡。
- **框架**：约束马尔可夫决策过程（CMDP），将安全需求编码为代价信号，而非硬编码规则。
- **仿真环境**：NVIDIA Isaac Sim 中的双 KUKA iiwa 机械臂，支持并行化训练与真实的接触动力学，
  便于研究双臂协同。

## 当前进展

该项目仍在进行中，后续会持续更新研究细节、实验结果，以及可能产出的论文。

## 相关工作

本项目延续了此前课程项目中开发的方法，参见
[基于 Lagrangian SAC 的孔轴装配安全强化学习](/zh/research/peg-in-a-hole-lagrangian-sac/)。
