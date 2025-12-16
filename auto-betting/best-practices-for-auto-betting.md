---
icon: vest-patches
cover: ../.gitbook/assets/abdocs.png
coverY: 0
---

# Best Practices for Auto-betting

Auto-betting is a powerful execution tool, but it is **not magic**.

Because it is **highly configurable**, the quality of replication depends heavily on how you set it up. If your settings are too strict (or inconsistent with the tipster’s style), the system may:

* skip many tips,
* or reject bets because your limits are reached.

{% hint style="warning" %}
Auto-betting replicates tips **only when your own rules allow it**. Configuration is the user’s responsibility.

If you’re unsure how to configure your strategy, you can reach out to us and we will help you choose sensible settings.
{% endhint %}

Before reading this page, make sure you understand:

* [What is Auto-betting?](what-is-auto-betting.md)
* [How Auto-betting Works](how-auto-betting-works.md)
* [Auto-betting Requirements & Limits](auto-betting-requirements-and-limits.md)

***

### 1) Treat auto-betting like an investment process

Auto-betting should be approached the same way as bankroll management:

* define stable rules
* avoid emotional changes
* judge performance on enough volume

This is the same philosophy described in [Best practices](../bankrolls/best-practices.md).

{% hint style="info" %}
Auto-betting does not remove variance — it removes **execution friction**.
{% endhint %}

***

### 2) Start conservative (then scale)

If you are new to auto-betting, don’t start by following 10 tipsters with aggressive stakes.

A safer ramp-up is:

1. start with **2–3 Experts**
2. configure max stake per day per tipster to 3-4 units
3. configure max stake per day to 10 units&#x20;

***

### 3) Use units consistently (and convert them correctly)

Most long-term strategies work best with consistent staking.

On Bet2Invest, Experts typically publish in **units**. In auto-betting, you convert those units into currency using:

* **Stake per unit** (your currency value for 1 unit)

Then protect yourself with:

* **Max stake per unit** (hard cap)
* **Max stake per day per tipster** (exposure cap)

{% hint style="danger" %}
Don’t increase your stake per unit because you “feel confident” about a tipster. If you want higher stakes, increase slowly and keep daily / per-tipster caps.
{% endhint %}

If you need a refresher on units, read [What's a Unit?](../bankrolls/whats-a-unit.md).

***

### 4) Configure odds protection (slippage control)

The most common reason auto-betting “doesn’t replicate well” is simple: **odds move**.

To control slippage, your key setting is:

* **Max odds drop (%)**

Guidance:

* Too low → you will miss many tips.
* Too high → you may copy after the value is gone.

Also consider your **order type**:

* **Market (instant)** — best replication, but more sensitive to fast moves.
* **X minutes before market closure** — useful for specific strategies where CLV is negative, but can create large differences vs the tipster’s entry.
* **Only if price rises again after drop** — can reduce chasing bad prices, but can also reduce fill rate.

{% hint style="info" %}
There is always a trade-off between **fill rate** (placing more bets) and **price quality** (avoiding bad odds).
{% endhint %}

***

### 5) Respect liquidity (especially on niche markets)

Liquidity affects how easily odds move.

* High-liquidity markets (top leagues, main lines) usually replicate better.
* Low-liquidity markets (niche leagues, props, derivatives) can move fast and create more rejections or slippage.

This matters even more when many followers copy the same tip.

To understand liquidity basics, see [Best practices](../bankrolls/best-practices.md).

***

### 6) Prefer diversification over overconfidence

If you put all your exposure on one tipster, your variance and risk increase.

Better habits:

* follow a small set of Experts with different sports / styles
* keep **per-tipster daily caps**
* avoid stacking multiple tipsters who bet the exact same markets at the same time

{% hint style="success" %}
Diversification is one of the simplest ways to reduce variance risk.
{% endhint %}

***

### 7) Monitor failures and adjust (without over-optimizing)

Some bets will fail. That’s normal.

Common causes:

* market closed
* odds moved beyond your max odds drop
* Pinnacle rejected the bet
* your daily / per-tipster cap was reached

Best practice is to:

* review your acceptance vs rejection rate
* identify which rule is causing most misses
* adjust only if it matches your strategy goals (replication vs price quality)

{% hint style="warning" %}
Don’t change your rules every day. Treat configuration like a strategy: stable rules, review on meaningful samples.
{% endhint %}

***

### 8) Evaluate the right metrics (not only short-term profit)

Auto-betting makes execution consistent, so it becomes easier to evaluate a strategy.

When possible, focus on:

* long-term yield on enough volume
* CLV/CLEV (market beating signals)

Learn more here:

* [Why CLV & CLEV Matter](../bankrolls/why-clv-and-clev-matter.md)

***

### 9) Ask for help if you’re unsure

Auto-betting is designed to be flexible, and there is no single “best” configuration.

If you tell us:

* your bankroll size
* your target monthly risk
* whether you prefer prematch or live
* how many Experts you want to follow

…we can suggest safe, realistic settings.
