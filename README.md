# Dash Incubator Bounty Protocol

This document describes the protocol and incentive structures related to the Dash Incubator bounty program.  Dash Incubator is a multi-phase project funded by the [Dash superblock](https://docs.dash.org/en/stable/governance/understanding.html).  Past and current phases are as follows:

* Phase 1 proposal (complete) - [Dash Nexus](https://app.dashnexus.org/proposals/dash-platform-incubator/overview) | [Dash Central](https://www.dashcentral.org/p/dash-platform-incubator)
* Phase 2 proposal (complete) - [Dash Nexus](https://app.dashnexus.org/proposals/dash-platform-incubator-phase-2/overview) | [Dash Central](https://www.dashcentral.org/p/dash-platform-incubator-phase-2)
* Phase 3 proposal (current) - [Dash Nexus](https://app.dashnexus.org/proposals/dash-platform-incubator-phase-3/overview) | [Dash Central](https://www.dashcentral.org/p/dash-platform-incubator-phase-3)

## Background description

> description of Dash Incubator taken from a comment by Andy in the [phase 3 proposal](https://www.dashcentral.org/p/dash-platform-incubator-phase-3) - unedited for now, can update in later commit and remove this comment.

The incubator is a fund that redistributes block rewards repackaged as 1-time incentives to people who chose to produce or facilitate the production of units of open-source output focused on Evolution such as Dapps, tools, tutorials, sample code running on L2. The only structure is a protocol of how those incentives are selected and offered and how the resulting work is validated so the funds are awarded to the people who produce that output.

It's informal right now but i'm working on formalizing this protocol in a github repo with some of the other devs... but the general ethos has assumptions such as no fixed costs or hierachies that can't rapidly adapt to change, everything is open, all work is by choice, people work when they want, all work is competitive, and all work is incentivized. Developers work best when they are having fun and building what they see value in. Sometimes devs are busy and sometimes not, sometimes they want to work on different things or try different 'roles', all devs want to build positive cred and reputations through output. By having all work modularized and task based and basically a market place for work with everything transparent it provides a lot of freedom and creativity... it's a new thing i'm trying and really antithetical to any traditional corporate structure, and it's only possible on a completely remote-based and decentralized network funded model and it's working really well.

There's funds and a protocol - the people involved at any one time are fluid, it's just people incentivized to define work, complete work, QA work through pipeline defined by that protocol (currently working across tools like Trello, Pivotal, GDocs) - but no one is contracted, permanent, or officially positioned or able to present as any kind of team (just me behind it with a private key paying addresses that are QA'd and that will be decentralized ultimately too). It's a different tool for a different job than DCG.

## Process & protocol

### Current process

> description of current process as interpreted by Rion - to document the history and use as a basis for disucssing proposed changes, can remove this section (or at least this comment) later.

The current process for administering bounties is somewhat informal:  Typically, the process goes something like this:

1. Someone comes up with an idea that potentially falls within the scope of Dash Incubator.
2. That idea finds its way to the person working on the [bounty admin meta-bounty](https://trello.com/c/Sg59jrBr/52-bounty-admin) - previously @readme, currently @rion - by either a) the idea originator directly contacting the admin or Andy, or b) the admin or Andy seeing the idea crop up on one of the Dash forums.
3. The admin (or Andy) makes a card on the [Trello bounty board](https://trello.com/b/FPJzDcok/dash-bounty-board).
4. The admin (or Andy) works with the idea creator and any other interested devs to add specifications, turning the idea into a bounty (with a scope, tasks, bounty amounts, etc.).
5. Someone asks to "reserve" the bounty for themselves (often the originator of the idea).  This is useful so that multiple people aren't working on the same bounty at the same time, knowingly or not.
6. Eventually the developer completes one or more of the specified tasks in the bounty and makes a claim showing the work completed and giving an address for payment.
7. The bounty admin checks the work, verifies that it satisfied the description, and informs Andy to award the bounty.
8. Andy pays the developer.
9. The claims are documented on the [bounty claims Google sheet](https://docs.google.com/spreadsheets/d/1mhXlo4ylqWLLSYN4MGiLWlp7Gq3jrsDt0kB701dwMNU/edit#gid=0).

### Proposed protocol

The bounty lifecycle described above has worked well for the past and present size, but for Dash Incubator to scale effectively and efficiently, the 'informal process' needs to be transformed into a 'formal protocol', such that it can eventually be implemented as a decentralized app on Dash Platform itself.  Furthermore, in order to keep the bounty pipline flowing, financial incentives need to be added to more steps of the bounty lifecycle.

The structure and incentive transition will be gradual, moving from centralized tooling to decentralized tooling as appropriate for the needs and focus of the fund.  The incubator is focussed on code output (particularly Dash Platform data contracts), not administration. The transition aims to incentivize code output (quantity and quality), and reduce administrative barriers and overhead.

> The following sections are the ideas I (Rion) shared in the [dummy Trello board](https://trello.com/b/WEfG7f9Q/dash-incubator) - mostly unedited for now, just placeholders to be updated in later commits, removing this comment and parts of the previous descriptive paragraphs.  The ideas is for bounties to have a certain 'state' at any point - proposed, confirmed, specified, coded, tested, paused, completed.

#### Proposing a bounty

Anyone can propose a bounty idea to put it up for consideration. If you are already on Trello, just add a card to "Imagined" using the provided template. If you are not on Trello, ask someone who is to add your idea

#### Confirming a bounty

A bounty that makes it here will eventually yield 5% (of the bounty reward) to the person who approved it (the Admin - Rion at this point - but could be decentralized later).  For now, approving a project is a matter of authority (Andy authorizes Rion to do this).  The incentive to approve bounties is 5% of the reward, the disincentive to approve small, dumb projects is that it adds overhead and your reputation could suffer.

#### Specifying a bounty

Specifying a project means defining tasks, requirements, technologies, and tests related to the bounty.  It's putting flesh on the bones of what was imagined for the bounty, how it intended to add value.  This step is critical for successful coding.

#### Coding a bounty

This is the meat of the bounty.  This is our product, our output, our value - open source code.  The code must satisfy both the letter and the spirit of the bounty specification law.

#### Testing a bounty

Testing a bounty is straight forward going through the motions of performing the testing requirements spelled out in the bounty specification.  For now this will be done by the Admin, Rion, but can be decentralized later.

#### Pausing a bounty

A bounty can be paused for several reasons:

* the developer who reserved the bounty gets busy
* the developer is waiting on someone stalling the critical path of interdependent bounties
* the bounty is renewable (a phase is complete and awaiting new tasks to be specified)
* etc.

#### Completing a bounty

A bounty is completed if it is not renewable - a phase is complete and no new tasks can be imagined to recycle it back to the west where it will recommence it's journey eastward.

## Resource list

* Dash Incubator bounty board - [Trello](https://trello.com/b/FPJzDcok/dash-bounty-board)
* Dash Incubator bounty claims - [Google sheet](https://docs.google.com/spreadsheets/d/1mhXlo4ylqWLLSYN4MGiLWlp7Gq3jrsDt0kB701dwMNU/edit#gid=0)
* Dash Incubator bounty fund - [Dash insight](http://insight.dash.org/insight/address/XbFb9b1qaoLykngDbUwBVBFwSHuwQRhSqc) | [Blockchair](https://blockchair.com/dash/address/XbFb9b1qaoLykngDbUwBVBFwSHuwQRhSqc)
* Dash developer public chat - [Discord](https://chat.dashdevs.org/)
