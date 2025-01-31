---
title: 持续集成 (CI)
status: Completed 
category: 概念
---

## 是什么

持续集成，通常缩写为CI，是尽可能定期集成代码变化的做法。
CI 是 [持续交付](/zh-cn/continuous-delivery/)（CD）的前提。
传统上，CI 过程从代码修改提交到源码控制系统（Git、Mercurial 或 Subversion）时开始，以准备被CD系统使用的测试工件结束。

## 解决的问题

软件系统通常是庞大而复杂的，有许多开发人员在维护和更新它们。
在系统的不同部分平行工作，这些开发人员可能会做出相互冲突的修改，并在无意中破坏对方的工作。
此外，由于多个开发人员在同一个项目上工作，任何日常工作，如测试和计算代码质量，都需要由每个开发人员重复进行，浪费了时间。

## 如何帮助

每当开发人员提交修改时，CI 软件都会自动检查代码修改是否合并得很干净。
使用 CI 服务器来运行代码质量检查、测试甚至部署，这几乎是一种普遍的做法。
因此，它成为团队内部质量控制的一个具体实施。
CI 允许软件团队把每一个代码提交变成具体的失败或可行的候选发布。
