---
icon: chart-waterfall
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

# Why CLV & CLEV Matter

CLV and CLEV are two of the most important metrics used on Bet2Invest to evaluate whether a strategy has a **repeatable edge**.

They are not perfect, but they are much harder to “game” than short‑term results, and they are widely used in sharp betting to assess whether someone consistently beats the market price.

{% hint style="warning" %}
**Important:** CLV and CLEV are _indicators_, not certainties. They have **not been formally “proved”** as guaranteed long‑term predictors, and we cannot be 100% sure they will always translate into long‑term profitability for every sport, market, or strategy.
{% endhint %}

***

### Definitions

#### CLV (Closing Line Value)

**CLV** compares the odds you took when you placed your bet to the **closing odds** (the final Pinnacle price right before the event starts).

Intuition:

* If you consistently take **better odds than the close**, you are “beating the market”.
* If you consistently take **worse odds than the close**, you are usually paying too much (at inefficient prices).

#### CLEV (CLV without the margin)

Odds include a bookmaker margin (vig). **CLEV** is a variant of CLV that removes the margin so the comparison focuses on the underlying market probability rather than the bookmaker’s edge.

On Bet2Invest, CLEV is used to better isolate **pure market efficiency**.

{% hint style="info" %}
In simple terms: **CLV tells you if you beat the closing price**; **CLEV tells you if you beat the closing price after removing the bookmaker margin**.
{% endhint %}

***

### Why CLV/CLEV are so important

#### 1) Results are noisy, CLV is a process metric

Short‑term yield is heavily impacted by variance:

* a good strategy can lose money for weeks
* a bad strategy can look “great” for 30–50 bets

CLV/CLEV measure the **quality of your entries**, not the outcomes of a small sample.

{% hint style="success" %}
Winning is not the same as having an edge. **Beating the closing line consistently** is often considered one of the strongest signs of edge in sports betting.
{% endhint %}

#### 2) The closing line is the best public benchmark

In sharp markets, the closing line reflects:

* the aggregation of information (injuries, lineups, motivation, weather…)
* liquidity and sharp action
* market efficiency improving over time

If your prices are better than the close over a large sample, it suggests your model/timing/information tends to be ahead of the market.

#### 3) It helps you build and refine strategies

CLV/CLEV are actionable:

* if your CLV is negative, you may need to bet earlier, change leagues, change market types, or stop chasing steam.
* if your CLV is positive but results are negative, it often means variance (or a sample that is still too small).

***

### How to interpret CLV/CLEV

There are multiple ways to express CLV. Regardless of the exact format, the interpretation is the same:

* **Positive CLV / CLEV** = you beat the market closing price on average.
* **Negative CLV / CLEV** = you take worse prices than the close on average.

#### What matters most

* **Sample size** – CLV becomes meaningful after **hundreds of bets**.
* **Liquidity** – low-liquidity markets move more and can make CLV easier to achieve but harder to scale.
* **Consistency** – stable, repeatable CLV is a stronger signal than occasional spikes.

To understand why liquidity matters, see [Best practices](best-practices.md).

***

### Common misconceptions (important)

#### “Positive CLV guarantees profit”

No. Even with a real edge, you can run bad for a long time.

CLV increases the probability of long‑term profitability, but it does not remove variance.

#### “CLV is everything”

Also no. CLV can be misleading if:

* you bet markets with **very low liquidity** (easy to move)
* you cherry-pick markets or timing in a way that can’t be replicated

Bet2Invest therefore looks at CLV/CLEV alongside other indicators (volume, yield, drawdown, liquidity…).

***

### How this fits into Bet2Invest

When you place bets inside a Bet2Invest bankroll, the platform can later compute:

* the **closing odds** on Pinnacle
* your **CLV** and **CLEV**
* additional market context (margin, line movement, etc.)

This is one of the reasons Bet2Invest relies on Pinnacle as a reference: it makes strategies comparable on a consistent and efficient market.

If you haven’t yet, see [Analyze Pinnacle Markets](../getting-started/get-started/analyze-pinnacle-markets.md) to understand how to browse markets and start tracking your own.
