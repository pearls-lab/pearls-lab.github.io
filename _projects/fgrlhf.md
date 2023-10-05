---
layout: page
title: Fine-grained Natural Feedback
description: How to build better rewards, i.e. proxy models of human preferences?
img: assets/img/fgrlhf-mini.png
importance: 2
category: Human Preference Alignment
related_publications: wu2022inscit, wu2023finegrained
---

Currently the prevailing form of human preference data collection is as thus: humans are presented with two or more outputs and asked to select one or rank them. 
This signal is then used to train a reward model, which computes a single scalar reward for each LM-generated
sequence. 
The LM is then trained with RL to optimize the reward it receives (from the reward model). Such a reward provides a relatively sparse training signal, especially for tasks that require the
generation of long-form text—making RLHF in such domains unreliable.
This project focuses on what it would take to move towards more natural (language), fine-grained rewards along various dimensions.
