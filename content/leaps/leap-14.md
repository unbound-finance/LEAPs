---
leap: 14
title: Reimburse LYRA to LPs
status: Implemented
author: jake (@earthtojake)
created: 2022-01-12
---

<!--You can leave these HTML comments in your merged LEAP and delete the visible duplicate text guides, they will not appear and may be helpful to refer to if you edit it again. This is the suggested template for new LEAPs. Note that a LEAP number will be assigned by an editor. When opening a p ull request to submit your LEAP, please use an abbreviated title in the filename, `leap-draft_title_abbrev.md`. The title should be 44 characters or less.-->

## Simple Summary
<!--"If you can't explain it simply, you don't understand it well enough." Simply describe the outcome the proposed changes intends to achieve. This should be non-technical and accessible to a casual community member.-->
Core contributors discovered a bug in the off-chain script used to calculate LYRA rewards for LPs of market pools. This resulted in 179,332 LYRA being distributed incorrectly. This LEAP proposes that LPs are reimbursed the 179,332 LYRA in the upcoming token distribution on Fri Jan 14 2022 07:00 UTC. These tokens will come from the [Liquidity Rewards distribution](https://leaps.lyra.finance/leaps/leap-7#4-liquidity-rewards-15).

## Abstract
<!--A short (~200 word) description of the proposed change, the abstract should clearly describe the proposed change. This is what *will* be done if the LEAP is implemented, not *why* it should be done or *how* it will be done. If the LEAP proposes deploying a new contract, write, "we propose to deploy a new contract that will do x".-->
The bug in question can be found in the [lyra-lp rewards script](https://github.com/lyra-finance/lyra-scripts/blob/master/src/rewards/lyra-lp/getLyraLPRewards.ts). LPs who requested withdraw but did not execute their withdraw before the next round started were still included in reward distribution for the next round, despite their liquidity not being locked in the pool.
Over the 5 rounds of liquidity provision for markets, this accounted for misallocation of 179,332 LYRA, meaning some LPs were over and under-rewarded.
This LEAP proposes that under-rewarded LPs are reimbursed the 179,332 LYRA and that over-rewarded LPs are not slashed or penalized in any way (as it is impractical to do so). LPs will be reimbursed in the upcoming token distribution on Fri Jan 14 2022 07:00 UTC from the [Liquidity Rewards distribution](https://leaps.lyra.finance/leaps/leap-7#4-liquidity-rewards-15).


##  Motivation
<!--This is the problem statement. This is the *why* of the LEAP. It should clearly explain *why* the current state of the protocol is inadequate.  It is critical that you explain *why* the change is needed, if the LEAP proposes changing how something is calculated, you must address *why* the current calculation is innaccurate or wrong. This is not the place to describe how the LEAP will address the issue!-->
LPs that were under-rewarded deserve their fair share of rewards for providing liquidity.

## Specification

<!--The specification should describe the syntax and semantics of any new feature, there are five sections
1. Overview
2. Rationale
3. Technical Specification
4. Test Cases
5. Configurable Values
-->

### Overview
<!--This is a high level overview of *how* the LEAP will solve the problem. The overview should clearly describe how the new feature will be implemented.-->
The script used to calculate rewards will be modified to determine how much each LP was under-rewarded in past rounds. A distribution event will be created specifically for under-rewarded LPs. The bug will be fixed for all future rounds. These changes will be published to the [lyra-lp rewards script](https://github.com/lyra-finance/lyra-scripts/blob/master/src/rewards/lyra-lp/getLyraLPRewards.ts).

### Configurable Values
<!--Please list all values configurable under this implementation.-->
179,332 LYRA was misallocated and will be rebistributed to LPs.

## Copyright
Copyright and related rights waived via [CC0](https://creativecommons.org/publicdomain/zero/1.0/).
