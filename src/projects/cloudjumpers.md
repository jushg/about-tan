---
title: Cloud Jumpers
date: 2022-04-06
repo: CloudJumpers/CloudJumpers
topics: ["Swift", "Django", "Game"]
lead: 1-4 players Platformer Game on IpadOS.
image: cloudjumper.png
---

An IpadOS platformer game for 1-4 players, built as part of CS3217 Team Project and won 1st Prize at NUS 20th STEPS.

I designed and implemented the event-based synchronisation pipeline for this project. This is to de-conflict the actions of different players (e.g. when 2 players try to obtain the same object at the same time). The system is developed using a central remote server as the single source of truth for all iPad clients, with priority queue using timestamp for priorisation of actions processing.


**Links: [GitHub](https://github.com/CloudJumpers/CloudJumpers),
[Documentation](https://github.com/jushg/CloudJumpers/blob/main/docs/Cloud%20Jumpers%20Final%20Report.pdf)**