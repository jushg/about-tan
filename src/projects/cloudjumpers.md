---
title: Cloud Jumpers
date: 2022-04-06
repo: CloudJumpers/CloudJumpers
topics: ["Swift", "Django", "Game"]
lead: 1-4 players platformer Game on IpadOS.
image: cloudjumper.png
---

Built as part of CS3217 (Software Engineering on Modern Application Platforms) team project.
We won 1st Prize at NUS 20th STEPS.

I implemented the event-based synchronization pipeline for this project. This is to deconflict the actions of different players (e.g. when 2 players try to obtain the same object at the same time). The system is developed using a central remote server as the single source of truth for all iPad clients, with priority queue using timestamp to rank which action to process.

I also designed the Game Engine API based on the Entity-Component-System (ECS) architecture, making it easily extensible
for future development of new game modes and game features.

**Links: [GitHub](https://github.com/CloudJumpers/CloudJumpers),
[Documentation](https://github.com/jushg/CloudJumpers/blob/main/docs/Cloud%20Jumpers%20Final%20Report.pdf)**