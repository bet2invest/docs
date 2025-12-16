---
icon: flag-checkered
cover: ../.gitbook/assets/experts.png
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

# How Picks Are Settled

Bet2Invest settles (grades) tips **automatically** using **official results from Pinnacle**.

This ensures that results are **consistent**, **timestamped**, and based on the same source used for the market data.

<figure><img src="../.gitbook/assets/Screenshot 2025-12-16 at 15.42.01.png" alt=""><figcaption></figcaption></figure>

***

### How settlement works

When an event finishes, Bet2Invest:

1. Retrieves the **official result** for the event from Pinnacle.
2. Applies the relevant settlement logic based on the market type (for example: final score, number of points/goals/sets, etc.).
3. Marks the tip as one of the standard outcomes (for example: **Won**, **Lost**, **Refunded**, or **Voided** where applicable).

{% hint style="info" %}
For the underlying grading definitions (refunds, cancellations, rescheduled events, etc.), Bet2Invest aligns with [Pinnacle betting rules](https://www.pinnacle.com/en/future/betting-rules).
{% endhint %}

***

### How long does it take?

Most tips are settled within **5 minutes to a few hours** after the event is finished.

Delays can happen, for example when:

* the event is not marked as “final” yet
* official data is delayed
* a market requires extra confirmation (cancellations, abnormal endings, etc.)

{% hint style="success" %}
In normal conditions, you don’t need to do anything—settlement is fully automatic.
{% endhint %}

***

### Cancellations, postponements, and abnormal endings

If an event is cancelled, postponed, or otherwise not completed as expected, the tip outcome is determined automatically based on the official status and grading rules.

Typical outcomes you may see:

* **Void / Cancelled**
* **Pending** (until the official status changes)

<figure><img src="../.gitbook/assets/Screenshot 2025-12-16 at 15.44.35.png" alt=""><figcaption></figcaption></figure>

***

### What if there is an error?

While settlement is automated, **errors can happen** (for example: incorrect official status, late corrections, or edge cases).

When this occurs:

* our admins can review the settlement
* incorrect settlements are **fixed** once identified

{% hint style="info" %}
Bet2Invest tips are meant to be immutable (selection/odds/stake history). Admin interventions are limited to fixing **clear issues** such as a settlement bug or incorrect grading.
{% endhint %}

{% hint style="warning" %}
If you believe a tip has been settled incorrectly, contact support with:

* event name
* market/selection
* the timestamp of the tip
* what you believe the correct settlement should be

This allows the team to verify it quickly.
{% endhint %}
