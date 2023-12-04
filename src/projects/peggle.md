---
title: Peggle Redux
date: 2022-02-03
repo: jushg
topics: ["Swift", "Realm", "Game"]
lead: iPadOS game with a physics engine that I built from scratch.
image: peggle.png
---

Built as part of CS3217 individual project, this is a clone of the 
famous Peggle game, complete with a Physics Engine and a Game Engine that I designed and implemented.

Game Engine is built follow the Entity-Component-System architecture, and Physics Engine rely on the Separating Axis Theorem for collision checking and resolution between different objects

Beside Realm (ORM), which is used for persistence, no other external library is used for Physics Engine or Game Engine. Everything is created from scratch.


**Note: Currently the codebase is set to private to prevent code copying, please send me a message if you want to take a look.**

<!-- **Links: [GitHub](https://github.com/jushg/CloudJumpers),
[Crates.io](https://crates.io/crates/bore-cli),
[Documentation](https://docs.rs/bore-cli)** -->