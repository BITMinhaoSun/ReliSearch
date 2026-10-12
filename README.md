# ReliSearch

**Search When Needed, Proceed When Reliable: Metacognitive Reliability Monitoring for Efficient Agentic Search**

> **Code coming soon.** We are organizing the code and will release it in this repository.

## Overview

ReliSearch is a metacognitive framework for training language models to **search when external evidence is needed and proceed when their current information is sufficiently reliable**.

Final-answer correctness alone does not tell us whether a search decision was appropriate: a correct answer may come from a lucky guess, while a successful reasoning trajectory may contain unnecessary searches. ReliSearch addresses this performance-reliability mismatch by supervising the reliability of intermediate conclusions.

<p align="center">
  <img src="assets/intro.png" alt="Decision matrix illustrating appropriate search and no-search decisions, under-search, and over-search." width="800">
</p>

*Motivation: under-search proceeds from an unreliable state; over-search retrieves despite sufficient reliability.*

## Framework

<p align="center">
  <img src="assets/framework.png" alt="ReliSearch framework: agent rollouts, training-time reliability supervision, GRPO policy updates, and inference with the learned policy." width="1100">
</p>
