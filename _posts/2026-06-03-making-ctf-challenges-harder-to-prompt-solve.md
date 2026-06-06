---
title: Making CTF Challenges Harder To Prompt-Solve
date: 2026-06-03 18:00:00 -0500
categories: [CTF, Security]
tags: [ctf, ai, challenge-design, education]
description: AI assistance changes CTF design, but it does not have to make challenges worse.
---

AI changes CTF solving, but it does not remove the need for good challenge design.

The mistake is treating AI use as something you can reliably police. Most of the time you cannot. A better goal is to make blind prompting less effective while making real understanding more rewarding.

## Make The Challenge Specific

Generic challenges are easy to prompt-solve because the prompt contains the whole problem. If the challenge is simply "JWT alg none" or "basic SQL injection," the model has seen that pattern thousands of times.

Specific challenges age better. Add custom behavior, per-team state, odd parser logic, service interaction, unusual data formats, or a small chain that requires observing what this exact system does. The solver can still use AI as a tool, but they have to bring evidence back from the target.

## Require Artifacts, Not Just Answers

A final flag is easy to paste. A solve path is harder to fake.

Intermediate artifacts help: recovered keys, crafted payloads, decoded formats, screenshots of local evidence, exploit scripts, or a short writeup that explains why the bug exists. These do not have to turn the event into homework, but they help prize review and make the challenge feel more like real security work.

## Randomize The Right Things

Per-team secrets, salts, generated databases, unique containers, or instance-specific flags can keep shared AI output from becoming a universal answer. The trick is to randomize the data without randomizing the lesson. Every team should solve the same idea, even if their exact values differ.

## Keep It Fair

AI-resistant should not mean hostile. The point is not to punish beginners for using modern tools. The point is to design challenges where tools assist the process instead of replacing it.

A good challenge still gives the player enough evidence to reason from. It just asks them to reason from the actual artifact in front of them.
