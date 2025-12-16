---
icon: ticket
cover: ../.gitbook/assets/bankrolls.png
coverY: 0
layout:
  width: default
  cover:
    visible: true
    size: hero
  title:
    visible: true
  description:
    visible: true
  tableOfContents:
    visible: true
  outline:
    visible: true
  pagination:
    visible: true
  metadata:
    visible: true
---

# What's a Unit?

A **unit** is the universal way to measure bet size on Bet2Invest.\
It replaces currency to keep everything consistent and comparable between users and strategies.

Units allow you to track performance with stability, without being affected by emotional changes in stake size or differences in bankroll size.

***

#### Why Units Matter

{% columns %}
{% column width="50%" %}
**Consistency**\
Units force stable staking.\
No more random bet sizes or emotional “big bets.”
{% endcolumn %}

{% column width="50%" %}
**Comparability**\
Two bettors with different bankrolls can compare performance using the same unit scale.
{% endcolumn %}
{% endcolumns %}

1 unit is not a fixed amount of money.\
It is a **percentage of your bankroll**, defined by you.

{% hint style="info" %}
Most of the time, **we consider 1 unit should be equal to 1% of your bankroll.**

If your bankroll is $1000, your unit should be $10.
{% endhint %}

{% hint style="info" %}
By default, stakes can be selected in **0.25U increments** (0.25, 0.5, 0.75, 1, … up to 10).\
See [Unit Increments & Limits](unit-increments-and-limits.md).
{% endhint %}

***

#### How Units Work

{% stepper %}
{% step %}
### You Set Your Bankroll

Example: 1,000 euros.\
This is the base for defining your unit value.
{% endstep %}

{% step %}
### You decide how much 1 unit represents

As mentioned earlier, we recommend 1% of your bankroll, but it can go up to 3%, although it increases the risks.
{% endstep %}

{% step %}
### All picks use units, not money

If a tipster posts “1U”, it means you stake 1% _(or the percentage you have determined)_ of YOUR bankroll, whatever its size.
{% endstep %}
{% endstepper %}

***

#### Why Bet2Invest Uses 1U by Default

Most strategies collapse because bettors change their stake sizes constantly or chase losses.\
Bet2Invest enforces **1U staking** for tipsters and bankrolls to ensure:

* clear, honest performance
* no leverage
* no manipulation of stats
* no illusion of higher profits through variable staking

{% hint style="warning" %}
Bet2Invest will not recommend an expert and will lower their [rating](../experts/rating-system.md) if they use excessively varying unit sizes.
{% endhint %}
