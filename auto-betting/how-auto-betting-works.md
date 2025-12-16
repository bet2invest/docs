---
icon: seal-question
cover: ../.gitbook/assets/abdocs.png
coverY: 0
---

# How Auto-betting Works

This page explains **how auto-betting executes tips technically and logically** — from the moment a tipster publishes a tip on Bet2Invest to the moment a bet is (or isn’t) placed on your **own Pinnacle account**.

For the high-level concept and important disclosures, read [What is Auto-betting?](what-is-auto-betting.md).

***

### First, what is an API?

API stands for **Application Programming Interface**.

In simple terms, an API is a tool that allows two applications to **communicate with each other automatically**, without human intervention.

In our case, it allows Bet2Invest to send betting orders to Pinnacle in an automated, secure, and compliant way.

{% hint style="info" %}
Pinnacle provides an **official, documented API** designed for automated integrations. Bet2Invest uses **only this official API** to place bets.
{% endhint %}

***

### Step-by-step execution flow

{% stepper %}
{% step %}
### Identify the affected users

When a tipster publishes a tip, Bet2Invest:

1. identifies users who **follow / subscribe** to that tipster,
2. keeps only users who have **enabled auto-betting** for that tipster.

Only those users continue to the next steps.
{% endstep %}

{% step %}
### Apply your limits and constraints

For each follower, we run an automatic filter based on the user’s configuration and limits, such as:

* maximum stake per tipster
* maximum stake per day (per tipster)
* any additional rules configured for that tipster (sports filters, market type, odds drop tolerance, etc.)

Only accounts that respect **all** personal rules move forward.
{% endstep %}

{% step %}
### Fair ordering of followers

Once the final eligible list is built, we determine an execution order.

The goal is to be fair and to reduce odds drops caused by many users betting at the same time.
{% endstep %}

{% step %}
### Apply your execution conditions (price, timing, market)

Each user may have personal execution conditions, for example:

* odds / price constraints (e.g., max odds drop)
* timing constraints (e.g., place instantly vs X minutes before market close)
* market type constraints (prematch, live, or both)

At this stage, two outcomes are possible:

* **Conditions not met yet** → the bet is placed **on hold** and may be executed later if conditions become valid.
* **Conditions met immediately** → the process continues instantly.
{% endstep %}

{% step %}
### Final check right before sending the order

When the system is about to place the bet, it performs a final validation:

* the market is still **open**
* the odds are still **within your constraints**
* the stake is still **allowed**
* daily limits are not exceeded

The bet is sent to Pinnacle **only if every condition is validated**.
{% endstep %}

{% step %}
### Place the bet via Pinnacle’s official API

To prove to Pinnacle that **you** (not Bet2Invest) are the person placing the bet:

* Bet2Invest uses **your Pinnacle identifiers**
* these identifiers are stored encrypted using **AES‑256** with a **unique IV (initialization vector)**
* they are never accessible in plain text by anyone at Bet2Invest

Then the order is transmitted to Pinnacle through the **official API**.

{% hint style="warning" %}
Bet2Invest does not place bets “in its own name”. Bets are placed on **your Pinnacle account**, with your credentials, through Pinnacle’s official interface.
{% endhint %}
{% endstep %}

{% step %}
### Handle the outcome (success or failure)

Two scenarios are possible:

#### ✅ Success: the bet is placed

Bet2Invest records and displays in your tracking:

* the odds obtained
* the stake
* the timestamp
* market information
* the final bookmaker response (e.g., accepted)

#### ❌ Failure: the bet is not placed

The bet may fail for typical reasons such as:

* market closed before execution
* odds moved beyond your allowed limits
* stake rejected due to Pinnacle limits
* your configured daily / tipster limits were reached

In all cases, you receive a clear status so you can understand what happened.
{% endstep %}
{% endstepper %}

***

### Where your control matters most

Auto-betting is powerful, but execution quality depends on how you configure it.

The most important parameters usually are:

* **stake per unit** and **max stake per unit**
* **max odds drop**
* **order type** (instant vs delayed)
* **market type** (prematch vs live)

For limits and eligibility details, see [Auto-betting Requirements & Limits](auto-betting-requirements-and-limits.md).
