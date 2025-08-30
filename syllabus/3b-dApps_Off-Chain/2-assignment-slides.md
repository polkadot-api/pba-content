---
title: dApps track assignment
description: Assignment description of the dApps track
---

# Assignment

---

## Staking Validator Reward Analyzer

---

## Basic staking concepts

- Validators: Candidates to author blocks <!-- .element: class="fragment" -->
- Stake: Amount of slashable tokens <!-- .element: class="fragment" -->
- Nominators: Support validators <!-- .element: class="fragment" -->
- Era: Every 24h a new validator set is elected <!-- .element: class="fragment" -->

Notes:

On module 6 (Polkadot) you will go through staking in-depth, with all considerations about economic incentives, alternative methods, trade-offs, etc.

This is just a small introduction to the topic. Refer to the Polkadot wiki to learn more about staking as part of the research, and explore the different pallets to complete the assignment.

---

## Problem statement

As a nominator, I have to select up to 16 validators I will nominate. My staking rewards (in DOT) depend on the performance of these validators.

<div class="fragment">

I want to:

- Identify which validators have received the most rewards to optimize my staking strategy.
- Compare validator performance over time.
</div>

Notes:

All the following info is explained in the Assignment README.

---

## Base Requirements

Build a tool that helps compare validators based on their reward.

- Displays the current validator set, ordered by performance. <!-- .element: class="fragment" -->
  - APY <!-- .element: class="fragment" -->
- Provides a way to view historical performance across past eras. <!-- .element: class="fragment" -->

---

## Rewards

You'll see that every validator:

- Might or might not be elected for each era. <!-- .element: class="fragment" -->
- Get "points" based on their work during each era. <!-- .element: class="fragment" -->
- The nominators get token rewards based on: <!-- .element: class="fragment" -->
  - Validator points. <!-- .element: class="fragment" -->
  - Proportion of the total stake for that validator. <!-- .element: class="fragment" -->
  - Commission config of that validator. <!-- .element: class="fragment" -->

---

## Grading criteria

<ul>
<li class="fragment">Implementation</li>
<li class="fragment">Code Quality</li>
<li class="fragment"><span style="font-size: 1.2em; font-weight: bold">README</span></li>
</ul>

Notes:

- **Implementation**
  - Correctness and accuracy of implementation
  - Evidence of using various techniques used in class
  - As close to production ready as possible
  - Integrate it with a working node
- **Code Quality**
  - Use of best practices and efficient code
  - Well documented, with considerations and compromises noted

---

## Bonus points

- Abstract business logic into SDK-like library
- Basic tests
- Integrate with Chopsticks, or other mocked chain.

---

## Format

- Any framework you like <!-- .element: class="fragment" -->
- Bear minimum usability <!-- .element: class="fragment" -->
  - Example https://bounties.usepapi.app
- README <!-- .element: class="fragment" -->

Notes:

- The repository is blank, just has the Assignment.
- We need to be able to run and use the dApp to correct it. Feel free to use any tool you'd like to quickly hack stuff, even v0 or similar.
- Please, add a README with some information about how to run your project, which parts you have completed, considerations and things you would've done better.

---

# Let's start hacking!
