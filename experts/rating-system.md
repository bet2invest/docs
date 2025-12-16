---
icon: percent
---

# Rating System

Bet2Invest uses a **unified rating system** to help you quickly understand how strong and reliable an Expert (tipster) is.

Instead of looking at dozens of metrics yourself, you can use the rating as a **shortcut** to compare Experts – while still having full access to detailed stats when you want to dig deeper.

For context on what an Expert is and how to analyse their bankrolls, see:

* [What's an expert?](whats-an-expert.md)
* [How to Analyse Bankrolls?](../follow-experts/how-to-analyse-bankrolls.md)

***

### 1. Rating scale and when it appears

Our rating is a **single grade between 0 and 5**:

* **0** = failed / not investable based on our rules
* **5** = excellent, highly reliable based on our metrics

To avoid ratings based on too little data:

* An Expert receives their **first rating at 200 tips**.
* Before 200 tips, you will **not** see a rating. You must rely on the raw stats and your own judgement.

{% hint style="info" %}
The rating is **always about behaviour over a large sample**, not about a short hot streak.
{% endhint %}

***

### 2. Why the exact formula is not public

The rating combines many factors into a single score.

To protect the integrity of the system and **prevent bad actors from gaming it**, the **exact calculation formula is intentionally kept secret**.

What this means:

* You **know which metrics matter** (listed below).
* You **do not know the exact weights or precise thresholds**.

This is by design:

* It makes it much harder to artificially optimise only for the rating while ignoring real performance or follower experience.
* It keeps the focus on **building a robust, scalable strategy**, which naturally leads to a better rating.

***

### 3. Key metrics used in the rating

The rating considers a wide range of statistics. The most important ones are:

1. **Yield / Average Odds (together)**
2. **Number of Bets**
3. **Units Variance (stake consistency)**
4. **Liquidity**
5. **CLV / CLEV**
6. **Flat Stakes Profits**
7. **Other secondary metrics** (less important but still used)

Below is a high‑level explanation of each one.

#### 3.1 Yield & Average Odds (work together)

* **Yield** measures profitability: profit in units / total staked units.
* **Average odds** indicate how volatile the strategy is.

We look at these **together**:

* A given yield is **more impressive** if it is achieved at **lower average odds** (harder to beat very efficient, low‑odds markets).
* Very high yield at extremely high odds may be **less sustainable** and more volatile.

In practice, stable positive yield over a large number of bets, with reasonable odds, is a **very strong signal**.

#### 3.2 Number of Bets

Sample size matters. A bankroll with only 50 bets tells you almost nothing.

* More bets → **more reliable** metrics and rating.
* The rating grows in confidence as the Expert reaches several **hundreds or thousands of bets**.

This is why we only start rating from **200 tips**.

#### 3.3 Units Variance (stake consistency)

On Bet2Invest, strategies are supposed to follow **flat or near‑flat stakes** (for example always 1 unit, or small controlled variations).

* **Flat stake = better** for the rating.
* Large, frequent stake changes (**high unit variance**) are seen as a risk and can hurt the rating.

This protects users against:

* Artificially boosted results by making a few very large bets.
* Emotional staking (chasing losses or over‑betting on “confident” picks).

To understand units, see [What's a Unit?](../bankrolls/whats-a-unit.md).

#### 3.4 Liquidity

A strategy is only useful if followers can **actually replicate it**.

We therefore incorporate **liquidity** (for example via AMB – Average Maximum Bet) into the rating:

* High liquidity markets → easier for many followers to get similar odds.
* Low liquidity, niche markets → great ROI may be difficult to copy in practice.

Experts who operate in **scalable, liquid markets** are rewarded, because their performance is more realistic for followers.

See [Best practices](../bankrolls/best-practices.md) for more on liquidity.

#### 3.5 CLV / CLEV

**CLV (Closing Line Value)** and **CLEV** (CLV without the bookmaker margin) measure whether an Expert consistently beats the market closing price.

* Positive CLEV is one of the **strongest indicators** of true edge.
* Even if short‑term results are unlucky, a strategy that beats the closing line over time is very promising.

#### 3.6 Flat Stakes Profits

We also look at the **profit in units** assuming **flat stakes** (for example, always 1 unit per bet), independent of any minor stake changes.

* This shows whether the strategy would still be profitable **without any staking tricks**.
* It is an important safety check against manipulation by changing stakes.

#### 3.7 Other, secondary metrics

The system also considers other metrics (less important individually) such as:

* Drawdowns and volatility patterns
* Distribution of odds
* And other proprietary checks

These help refine the rating but are **secondary** compared to the main metrics above.

***

### 4. Automatic 0 rating rules

Some situations are considered **automatic failures**, regardless of other metrics.

If either of these conditions is true:

* **Yield < 0%**
* **Flat stakes profit < 0 units** (strategy loses money with flat 1U staking)

Then the **rating is automatically set to 0**.

This ensures that:

* Strategies that are **not profitable at all** do not get a positive rating.
* Short‑term luck with strange staking cannot hide a fundamentally losing edge.

{% hint style="danger" %}
If an Expert’s yield is negative or their flat‑stake profit is below 0 units, their grade is **0**, no matter what other metrics say.
{% endhint %}

***

### 5. Sorting and how to use the rating

By default, **Experts are sorted by their rating**.

* Higher‑rated Experts appear **first** in lists.
* Lower‑rated or unrated Experts appear **later**.

You should use the rating as a **starting point**, not as the only decision factor:

1. Use the **rating** to quickly shortlist a few promising Experts.
2. Then open their bankroll(s) and review the detailed stats using the guidance in [How to Analyse Bankrolls?](../follow-experts/how-to-analyse-bankrolls.md).
3. Consider your own **risk tolerance, variance preferences, and favourite sports/markets**.

Handled correctly, the rating system helps you **focus your attention** on strategies that are both **statistically strong and realistically followable**, without needing to reverse‑engineer every metric yourself.
