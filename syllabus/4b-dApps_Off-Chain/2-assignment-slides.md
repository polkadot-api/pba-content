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

As a nominator, I have to select up to 16 validators I will nominate. My staking rewards depend on the performance of these validators.

<div class="fragment">

I want to:

- Identify which validators have received the most rewards to optimize my staking strategy.
- Compare validator performance over time. <!-- .element: class="fragment" -->

<div>

Notes:

All the following info is explained in the Assignment README.

---

## Base Requirements

Build a tool that helps compare validators based on their reward.

- Displays the current validator set, ordered by performance. <!-- .element: class="fragment" -->
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

## Possible Add-Ons

Notes:

Completing the base challenge, if properly done, is enough to pass the assignment, and each add-on will earn extra points.

Note that graders will value quality over quantity, so don't go overboard on add-ons. Don’t bite off more than you can chew.

---

### Find out the minimum staking amount per era

Notes:

Investigate how the minimum token amount required to earn staking is calculated per each era, and display the result.

---

### Connect with a wallet

Notes:

Integrate your dApp with a wallet of your choice (Browser extension, ledger device, WalletConnect, etc.) and let the user select an account from that wallet.

Use the selected account as a default for the other tasks that need an account.

---

### Determine if an address can nominate

Notes:

Not all accounts can nominate, particularly the ones who don't have enough tokens to bond into staking.

Given an account address, find out whether it can nominate or not.

---

### Show the current status of a nominator

Notes:

Given an account address, show the nomination status of that account.

- Is it nominating?
- How much has it bonded?
- Is it earning rewards?
- Which validators has it selected? Which validator has been active per era?

---

### Compare a nominator's performance to others

Notes:

Given an account address, add an option to show the performance of that nominator, and to compare its performance with other nominators in the current era.

---

### Fix a nominator’s rewards by managing the staking bag

Notes:

Not all nominators recieve rewards in every era. Active nominators are selected through staking bags.

For a given nominator not earning rewards, find out if it's something that can be easily fixed by managing the bag it's in, or by adding more stake.

---

### Check if an address is in the correct staking bag.

Notes:

As nominators compound their stake, they may end up in the wrong bag.

For a given nominator address find out if it's in a wrong bag.

As an extra, find all the nominators which are missplaced.

---

### Manage bonded amount

Notes:

Enable users to bond more tokens or unstake and unbond them, by creating and submitting the appropriate transaction.

---

### Allow me to nominate up to 16 validators

Notes:

Enable users to select up to 16 validators from the list, creating and submitting a transaction to update the selected validators.

---

### More?

Notes:

This list is meant as something to help you follow specific goals, but if you identify something that adds value and is interesting, you also can add your own.

---

## Grading criteria

- Implementation
- Code Quality

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
- Integrate with Chopsticks

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
