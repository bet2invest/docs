---
icon: bars-staggered
cover: ../.gitbook/assets/abdocs.png
coverY: 0
---

# Auto-betting Queue System

To protect replication quality (odds slippage, execution fairness, and market impact), Bet2Invest may cap the maximum number of auto-betting followers for certain Experts.

When an Expert is **full**, Bet2Invest uses a **queue system** so new users can still request access without having to constantly retry.

***

### Why a queue exists

Auto-betting is executed on real markets. When too many users copy the same Expert on low-liquidity markets, it can lead to:

* larger odds drops for late users
* more rejected bets (market moved, suspended, closed)
* unrealistic performance compared to what followers can actually replicate

A follower cap + queue is designed to keep execution **realistic and fair**.

***

### How it works (high level)

1. An Expert reaches the **maximum** number of auto-betting followers.
2. If you try to enable auto-betting for that Expert, you can join a **queue** instead.
3. When a spot becomes available (for example, someone disables auto-betting for that Expert), the system will offer the freed slot to users in the queue.

{% hint style="info" %}
The goal is to make access predictable and fair, while protecting market replication for all followers.
{% endhint %}

***

### What can cause a spot to open

A spot can become available when:

* an existing follower **stops** auto-betting that Expert
* a follower is removed from auto-betting access
* Bet2Invest updates the follower cap because liquidity conditions change

***

### Important notes

* Joining the queue does not guarantee immediate activation.
* Caps and queue behavior may vary depending on the Expert’s markets and liquidity.
* Even when you are active, replication is still subject to your own limits and to Pinnacle acceptance rules.

To understand why some bets may still not be placed, read [Auto-betting Requirements & Limits](auto-betting-requirements-and-limits.md).
