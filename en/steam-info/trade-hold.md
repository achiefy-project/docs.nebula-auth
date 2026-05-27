---
icon: timer
---

# Trade hold

Steam applies temporary restrictions, or holds, on **trades** and the **Market** to protect accounts. These restrictions can be triggered by different account actions and affect your ability to:

* send trades
* accept trades that include your items
* use the market

Current information is available on the official Steam support page: [Trade and Market Restrictions](https://help.steampowered.com/faqs/view/451E-96B3-D194-50FC).

***

### ⚙️ How the hold system works

All holds in Steam work **in parallel**.

This means:

* if several restrictions are active on the account, they **do not stack**
* the resulting hold is determined by the **longest active hold**
* a shorter hold does not cancel a longer one.

    If there are holds for 15 days and 2 days, the actual hold will be 15 days.

### Example

Imagine that several actions happened on the account:

* registration → 15 days
* enabling Steam Guard → 7 days

➡️ both restrictions start at the same time, but the effective hold is **15 days**

#### **Another example**

Imagine that you:

* disabled Steam Guard → 15 days
* 10 days passed
* enabled Steam Guard again → 7 days

➡️ From the moment Steam Guard is enabled again, you will have 7 days:

* 5 days remaining from disabling Steam Guard
* 7 days from enabling Steam Guard

Both restrictions apply to trades and the Market, so the restrictions will be removed 7 days after Steam Guard is enabled again.

***

### 📋 Main types of holds

Below are the main actions that cause restrictions. This is not a complete list, only the most common cases:

<table data-full-width="false"><thead><tr><th>Action</th><th>Duration</th><th>Scope</th></tr></thead><tbody><tr><td>Trade reversal, Trade-Protected</td><td>30 days</td><td>Trades + Market</td></tr><tr><td>Password reset, after 60+ days of inactivity</td><td>30 days</td><td>Trades + Market</td></tr><tr><td>Password reset</td><td>5 days</td><td>Trades + Market</td></tr><tr><td>Recovery through support, 60+ inactive</td><td>30 days</td><td>Trades + Market</td></tr><tr><td>Recovery through support</td><td>15 days</td><td>Trades + Market</td></tr><tr><td>Account registration</td><td>15 days</td><td>Trades + Market</td></tr><tr><td>Removing Steam Guard</td><td>15 days</td><td>Trades + Market</td></tr><tr><td>Enabling Steam Guard</td><td>7 days</td><td>Trades + Market</td></tr><tr><td>First purchase or top-up in a year</td><td>7 days</td><td>Market</td></tr><tr><td>Transferring mobile Steam Guard</td><td>2 days</td><td>Trades + Market</td></tr><tr><td>Changing nickname in Steam</td><td>2 <strong>hours</strong></td><td>Trades</td></tr></tbody></table>

***

### ✅ Summary

* all holds work **in parallel**
* final duration = **the longest active hold**
* short restrictions do not affect long ones

### ❓ Frequently asked questions

<details>

<summary><strong>Can changing the password impose restrictions?</strong></summary>

By itself, **changing the password** does not cause a hold. A hold is caused by a **password reset**, _Forgot password?_, if there has been no activity on your account for 60 days or more. Activity through the web version of Steam does not reset this period.

</details>

<details>

<summary><strong>If I traded with a person and they canceled the trade, will I also get a hold?</strong></summary>

No. The trade hold related to Trade-Protected cancellations applies only to the account that initiates the cancellation. If you received a trade offer and canceled it, the hold applies only to you. If another person canceled an offer you accepted, the hold applies only to them.

</details>

<details>

<summary><strong>Why can I still not trade even though 7 days have passed?</strong></summary>

Most likely, another longer hold is active on the account.

Check:

* whether the account was created recently
* whether Steam Guard was disabled
* whether a password reset was performed

Take into account both the date and the time. Restrictions are tied to the exact moment of the action and count full periods, such as 24 hours or 7 days.

</details>
