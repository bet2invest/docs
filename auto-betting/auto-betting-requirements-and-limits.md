---
icon: light-emergency
cover: ../.gitbook/assets/abdocs.png
coverY: 0
---

# Auto-betting Requirements & Limits

This page lists what you need to use auto-betting on Bet2Invest, and the practical limits you should understand before relying on it.

For the concept and key disclosures, see [What is Auto-betting?](what-is-auto-betting.md). For the technical flow, see [How Auto-betting Works](how-auto-betting-works.md).

***

### Requirements (what you must have)

#### 1) A Pinnacle account

Auto-betting works **only with Pinnacle**.

You must have:

* an active and funded Pinnacle account
* valid Pinnacle identifiers (used to place bets through Pinnacle’s official API)

Your credentials are stored encrypted (AES‑256 + IV). See [What is Auto-betting?](what-is-auto-betting.md).

{% hint style="info" %}
Don’t have a Pinnacle account yet? You can reach out to us and we can help you create one, with a **free trial** that includes **one subscription** plus some **offered auto-betting credits**.
{% endhint %}

#### 2) Auto-betting enabled for at least one Expert

Auto-betting is configured **per Expert**. Following an Expert does not automatically place bets.

You must explicitly enable auto-betting and set your rules for that Expert (stake, limits, filters…).

#### 3) A positive fee balance on Bet2Invest

Bet2Invest uses a balance on the platform to charge **auto-betting fees**.

{% hint style="warning" %}
This balance is used **only to pay fees**. It is not a betting bankroll and it is not transferred to Pinnacle. Your betting funds must be available directly on your Pinnacle account.
{% endhint %}

#### 4) Sufficient betting funds on your Pinnacle account

Auto-betting places bets on your own Pinnacle account. If your Pinnacle balance is too low, Pinnacle will reject the bet.

***

### Limits

Even if you enabled auto-betting, not every tip will necessarily result in a bet being placed. The system always respects your rules and the bookmaker constraints.

#### A) Your configuration blocks the bet

A bet will not be placed if it violates any of your settings, for example:

* **Max stake per unit** would be exceeded
* **Max stake per day (per tipster)** reached
* **Max odds drop** exceeded
* Stake is below the minimum authorized by Pinnacle
* market type not allowed (prematch vs live)
* sport not allowed
* your order type rules are not met yet (e.g., delayed placement)

#### B) Market timing & availability

A bet can fail if:

* the market closes before the system sends the order (it rarely happens, but it's not impossible)
* a live market changes state (suspended / reopened) while the order is being processed

{% hint style="info" %}
Live markets are faster and more volatile than prematch markets. Expect more rejections due to suspensions and rapid price moves.
{% endhint %}

#### C) Odds movement (slippage)

Odds can change between:

* the moment the Expert publishes the tip
* the moment your bet reaches Pinnacle

This is normal in betting markets, especially on low-liquidity markets or when many followers copy the same tip. Most of the time, the auto-betting users are the first to get the odds.

To protect you, auto-betting supports a **max odds drop** rule.

#### D) Liquidity-based follower limits

Market **liquidity** impacts how much money a market can absorb before odds move.

To reduce extreme odds drops and keep execution realistic, Bet2Invest may **limit the maximum number of auto-betting followers** that can copy certain Experts / markets, depending on liquidity.

If you can’t enable auto-betting for an Expert (or if availability is limited), this is usually to protect followers from poor replication and unrealistic results.

**Queue when an Expert is full**

When an Expert has reached the maximum number of auto-betting followers, new users can join a **queue**.

As soon as a spot opens, users in the queue can be activated.

Learn more here: [Auto-betting Queue System](auto-betting-queue-system.md).

#### E) Pinnacle limits / acceptance rules

Even if your configuration allows it, Pinnacle can still reject a bet due to:

* account-level restrictions
* market-specific constraints
* the price changing during the final acceptance

Bet2Invest cannot override Pinnacle rules. It can only send the order through Pinnacle’s official API.

***

### Built-in risk controls you should use

Auto-betting is powerful, but it should be treated like running an automated strategy.

At minimum, we recommend configuring:

* **Stake per unit** (your unit value in currency)
* **Max stake per unit** (hard cap if units vary)
* **Max stake per day per tipster** (prevents runaway exposure)
* **Max odds drop** (prevents copying after heavy moves)
* **Market type** (prematch vs live)
* **Sports filters**

For bankroll discipline, also read:

* [What's a Bankroll?](../bankrolls/whats-a-bankroll.md)
* [What's a Unit?](../bankrolls/whats-a-unit.md)
* [Best practices](../bankrolls/best-practices.md)

***

### Important disclaimers

* Auto-betting **replicates tips**; it does not guarantee you will get the exact same odds as the Expert.
* Auto-betting does not guarantee profit.
* Bet2Invest does not hold betting funds and does not place bets as a syndicate.

If you have questions about Pinnacle API endorsement, you can contact Pinnacle at `api@pinnacle.com`.
