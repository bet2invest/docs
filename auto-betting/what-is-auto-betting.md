---
icon: robot
cover: ../.gitbook/assets/abdocs.png
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

# What is Auto-betting?

Auto-betting on Bet2Invest is an automation feature that lets you **replicate Experts’ tips directly on your own Pinnacle account**, with rules you control.

It is similar to **copy-betting** (for now). In the future, it will evolve with more automation options and smarter execution features.

***

### What auto-betting does (and does not do)

#### What it does

When an Expert publishes a tip on Bet2Invest, auto-betting can:

* read the tip in real time
* check your personal constraints (stake, odds drop tolerance, market type, sport filters…)
* place the equivalent bet **on your own Pinnacle account**
* notify you with the final status (accepted / rejected / etc.)

#### What it does **not** do (important disclosure)

Auto-betting is **not** a betting wallet, a syndicate, or a fund.

* Bet2Invest does **not** hold any betting bankroll for you.
* Bet2Invest does **not** process bets internally.
* Bet2Invest does **not** act as a syndicate.

{% hint style="warning" %}
Your betting funds always stay on **your Pinnacle account**. The only link between Bet2Invest and Pinnacle is **technical** (execution through your account).

Deposits made on Bet2Invest (crypto / credit card) are used **only to pay auto-betting fees**, not to bet.
{% endhint %}

***

### Supported bookmaker

Auto-betting works **only with Pinnacle**.

This is intentional: Pinnacle is the reference market used across Bet2Invest (odds certification, market analysis, CLV/CLEV, liquidity…).

***

### Safety & compliance

#### “Is it safe for my Pinnacle account?”

Yes. Auto-betting is designed to be safe for your account and consistent with Pinnacle’s ecosystem.

* Auto-betting has been **officially endorsed by Pinnacle**.
* If you want official confirmation, you can reach out directly to Pinnacle: `api@pinnacle.com`.

#### Credentials & encryption

To enable auto-betting, you must enter your Pinnacle identifiers.

They are encrypted using **AES‑256** with an **IV** (initialization vector).

In simple terms:

* your identifiers are transformed into unreadable data before being stored
* even if someone accessed the database, the stored data would not be usable as plain text

***

### Fees (industry‑low)

Auto-betting fees are based on your plan:

* **Premium:** **0.2% ($0,20 for $100 volume)**
* **Standard:** **0.4% ($0,40 for $100 volume)**

Premium pricing:

* **€4.90 / month**
* **€49 / year**

{% hint style="success" %}
These fees are designed to be among the **lowest in the industry**, so automation stays accessible and scalable.
{% endhint %}

***

### Follow any Expert and define your own rules

You can enable auto-betting for **any Expert** you follow (PRO or not) and define a **different strategy for each Expert**.

For each Expert, you can configure:

* **Stake per unit**
* **Max stake per unit**
* **Max stake per day (per tipster)**
* **Max odds drop** (percentage)
* **Market type**: prematch, live, or all
* **Sports** filters
* **Order type** (how execution timing is handled):
  * **Market (instant)**
  * **X minutes before market closure** (X is configurable)
  * **Only if price rises again after a drop**

{% hint style="info" %}
This lets you follow multiple Experts while keeping strict bankroll discipline and execution constraints per strategy.
{% endhint %}

***

### Example: notification after a bet is placed

Below is an example of the message you can receive when auto-betting places a bet (translated to English):

```
➡️ Auto-betting: Bet placed ✅

📍 Bookmaker: Pinnacle
🏆 Event: Colorado Avalanche vs Florida Panthers (Hockey)
🏟️ League: NHL
📆 Match time: 12/12/2025, 02:37 AM
🎯 Market: Handicap (incl. OT): Florida Panthers +1.50 (1 Unit)

💰 Stake: $XXX
🏷️ Odds: 1.5
📉 Odds drop: 0.00%

😀 Tipster: XXX
📋 Unique ID: XXXXXX-XXXXX-XXXXXX-XXXXXXXX
⭐ Status: accepted

🔐 Your bet was placed successfully on your bookmaker.
```

***

### Deposits & bonus

Auto-betting uses a balance on Bet2Invest to pay execution fees.

* Deposits can be made by **crypto** or **credit card**.
* There is a **30% deposit bonus** on the balance (up to **€300** bonus).

{% hint style="warning" %}
This balance is for **fees only**. It is not used as a betting bankroll and it is not transferred to Pinnacle.
{% endhint %}

***

### Execution order (when many users copy the same tip)

When multiple followers are auto-betting the same Expert at the same time, execution order matters.

The subscription order between auto-betting followers is determined by:

* the follower’s **stake**
* the follower’s **reputation**
* the **age of the subscription**
* **random** order when the system cannot decide between users

This mechanism is designed to keep execution fair while accounting for real constraints.

***

### Next steps

* Follow the setup guide: [How to Set Up Auto-betting](how-to-set-up-auto-betting.md)
* Read [How Auto-betting Works](how-auto-betting-works.md)
* Review [Auto-betting Requirements & Limits](auto-betting-requirements-and-limits.md)
* For bankroll discipline, see [Best practices](../bankrolls/best-practices.md)
