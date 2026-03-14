---
icon: sparkle
---

# How to appear in the leaderboard?

The leaderboard highlights the top 5 tipsters of the moment, updated automatically based on your activity over the **last 30 days**. There is no manual curation: either you meet the criteria, or you don't.

***

### Eligibility criteria

To be considered for the leaderboard, you must meet all three conditions over the rolling 30-day window:

#### 1. At least 60 settled bets <a href="#id-1-at-least-60-settled-bets" id="id-1-at-least-60-settled-bets"></a>

You need a minimum of **60 settled bets** in the last 30 days. Pending or cancelled bets do not count. This threshold ensures the leaderboard only features tipsters with enough volume to produce statistically meaningful results.

#### 2. Flat yield ≥ 4 % <a href="#id-2-flat-yield-4" id="id-2-flat-yield-4"></a>

Your **flat-stake yield** must be at least 4 %. Flat yield is calculated as if every single bet was placed at exactly the same stake. This removes the influence of stake sizing and measures your raw picking edge.

{% hint style="info" %}
A flat yield of 4 % means that for every 100 bets at 1 unit, you return 4 units of profit.
{% endhint %}

#### 3. Consistent staking <a href="#id-3-consistent-staking" id="id-3-consistent-staking"></a>

The difference between your largest and smallest stake over the period must be **3 units or less**. You can vary your stakes slightly, but the spread must stay tight.

| Stakes used | Difference | Eligible |
| ----------- | ---------- | -------- |
| 1U – 3U     | 2          | ✅ Yes    |
| 1U – 4U     | 3          | ✅ Yes    |
| 1U – 5U     | 4          | ❌ No     |
| 7U – 10U    | 3          | ✅ Yes    |
| 5U – 10U    | 5          | ❌ No     |

This rule exists to ensure the leaderboard reflects genuine picking skill, not selective stake sizing.

### How ranking works

Among all eligible tipsters, the leaderboard is sorted by **flat-stake profit**; the total profit generated over the last 30 days at a flat stake.

$$
\text{Flat profit} = \text{Flat yield} \times \text{Number of bets}
$$

This means **volume and consistency are rewarded alongside yield**. A tipster with 200 bets at 4% flat yield (= 8U profit) ranks above one with 60 bets at 5% flat yield (= 3U profit).

| Tipster | Bets | Flat Yield | Flat Profit | Ranked |
| ------- | ---- | ---------- | ----------- | ------ |
| A       | 200  | 4%         | **8U**      | 🥇 1st |
| B       | 100  | 6%         | **6U**      | 🥈 2nd |
| C       | 60   | 5%         | **3U**      | 🥉 3rd |

### Summary

| Criterion                   | Requirement                |
| --------------------------- | -------------------------- |
| Settled bets (last 30 days) | ≥ 60                       |
| Flat yield (last 30 days)   | ≥ 4 %                      |
| Stake consistency           | Max − min stake ≤ 3U       |
| Ranking metric              | Flat profit (yield × bets) |
| Spots available             | Top 5                      |
