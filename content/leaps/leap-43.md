---
leap: 43
title: Kwenta Hosting Pilot
status: Draft
author: Leifu Chen (@LeifuChen), Burt Rock (@BurtRock)
created: 2022-12-30
---

<!--You can leave these HTML comments in your merged LEAP and delete the visible duplicate text guides, they will not appear and may be helpful to refer to if you edit it again. This is the suggested template for new LEAPs. Note that a LEAP number will be assigned by an editor. When opening a pull request to submit your LEAP, please use an abbreviated title in the filename, `leap-draft_title_abbrev.md`. The title should be 44 characters or less.-->

## Simple Summary
<!--"If you can't explain it simply, you don't understand it well enough." Simply describe the outcome the proposed changes intends to achieve. This should be non-technical and accessible to a casual community member.-->
This LEAP sets out the terms of a proposal by Kwenta DAO, requesting a pilot period allowing Kwenta DAO to host a front end for the Lyra protocol as part of the Kwenta exchange (kwenta.eth.limo) (Kwenta Interface) for a period of 6 months (Pilot). This Pilot requires Lyra DAO to provide: 
- A grant of up to 400,000 LYRA to Kwenta DAO to undertake the Pilot, to be paid linearly in monthly instalments (subject to Lyra DAO review throughout the Pilot); and
- Priority support from Lyra DAO Core Contributors, including weekly meetings, open ended sync communications channels and technical support for disruptions between the Kwenta Interface and the Lyra protocol.
Prior to the end of the Pilot, Kwenta DAO will provide a subsequent LEAP proposing the terms of any ongoing arrangement between Kwenta DAO and Lyra DAO.


## Abstract
<!--A short (~200 word) description of the proposed change, the abstract should clearly describe the proposed change. This is what *will* be done if the LEAP is implemented, not *why* it should be done or *how* it will be done. If the LEAP proposes deploying a new contract, write, "we propose to deploy a new contract that will do x".-->
This proposal introduces Kwenta DAO as the first third party interface deployer of the Lyra protocol. This will involve Kwenta hosting its own interface (the Kwenta Interface) that provides users with access to trade Lyra protocol sourced options for the Pilot period. Kwenta DAO and Lyra DAO Core Contributors will work together to support the Kwenta Interface connecting to Lyra protocol, with a view to determining longer term commercial arrangements subject to a successful Pilot.

## Motivation
<!--This is the problem statement. This is the *why* of the LEAP. It should clearly explain *why* the current state of the protocol is inadequate.  It is critical that you explain *why* the change is needed, if the LEAP proposes changing how something is calculated, you must address *why* the current calculation is innaccurate or wrong. This is not the place to describe how the LEAP will address the issue!-->
The Lyra protocol provides users with infrastructure to build and trade options. The Lyra DAO is focussed on back end development and support for clients building and hosting interfaces to access the Lyra protocol. 

In traditional finance, options trading is typically offered as a component of a suite of spot and derivatives trading tools and access to a broader range of financial instruments. However, the Lyra interface (as currently implemented) only provides a single venue for creating and trading options. 
There is an opportunity to expand the reach and use of the Lyra protocol by offering access to clients who can build tailored interfaces facilitating access to the Lyra protocol and offer trading activities together with other financial products and services not built on the Lyra protocol. 

Kwenta is a project focused on providing a user interface and tool suite to customers for a range of spot and derivatives offerings on Optimism. Kwenta is proposed as the first (pilot) user proposing to build and host an options trading interface. 

Providing third parties with access to the Lyra protocol and liquidity to support their product offerings will allow Lyra to maintain its core focus of growing a strong backend system rather than compete against providers that offer a range of financial services and instruments.


## Specification
<!--The specification should describe the syntax and semantics of any new feature, there are five sections
1. Overview
2. Rationale
3. Technical Specification
4. Test Cases
5. Configurable Values
-->
During the Pilot:

a) Lyra DAO’s role
Lyra DAO will provide Kwenta DAO with:
- Access to the Lyra interface to develop and host its own interface (the Kwenta Interface); 
- Access to the Lyra protocol to support the Kwenta Interface; 
- A grant of up to 400,000 LYRA to undertake the Pilot, to be paid linearly in monthly instalments (subject to Lyra DAO review throughout the Pilot); 
support from Lyra DAO Core Contributors, including weekly meetings, open ended sync communications channels and technical support for disruptions between Kwenta Interface and the Lyra protocol.

b) Kwenta DAO’s role
Kwenta DAO will:
- Develop and host the Kwenta Interface to be made available to Kwenta users on the Kwenta exchange (kwenta.eth.limo); 
- Deploy the Kwenta Interface to provide users with access to Lyra sourced options only; 
- Not charge any additional fees to users accessing the Lyra protocol through the Kwenta Interface;
- Not in any way indicate that it can bind Lyra DAO; 
- Only deal with the LYRA tokens provided in connection with the Pilot through staking, and will not ‘dump sell’ any LYRA tokens; 
prior to the end of the Pilot period, develop a subsequent LEAP proposing the terms of any ongoing commercial arrangement between Kwenta DAO and Lyra DAO with respect to the Kwenta Interface.

c) Other matters
This LEAP does not propose to limit any actions that can be taken by Lyra DAO in respect of the Lyra interface or the Lyra protocol. 

This arrangement is not intended to be exclusive and Lyra DAO may provide services to other parties providing interfaces with Lyra protocol. This LEAP is only to support a project proposed by Kwenta DAO to develop and operate a Lyra protocol integrated interface.

If engagement during the Pilot indicates that a longer term commercial arrangement with Kwenta DAO is not in the best interests of Lyra DAO, a disengagement plan will be agreed and implemented. 

Execution of this LEAP is subject to the Kwenta DAO approving a KIP on substantially similar terms to this LEAP. 

## Copyright
Copyright and related rights waived via [CC0](https://creativecommons.org/publicdomain/zero/1.0/).
