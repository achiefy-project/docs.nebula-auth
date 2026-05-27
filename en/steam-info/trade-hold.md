---
icon: timer
---

# Trade hold

Steam applies temporary restrictions, holds, on **trades** and the **market** to protect the account. These restrictions can arise from various account actions and affect the ability to:

* send trades
* accept trades that include your items
* use the market

Current information can be found on the official Steam support page: [Trade and Market Restrictions](https://help.steampowered.com/faqs/view/451E-96B3-D194-50FC).

***

### ⚙️ How the hold system works

All holds in Steam work **in parallel**.

This means:

* if several restrictions are active on the account, they **do not stack**
* the resulting hold is determined by the **longest active hold**
* the shorter period does not cancel the longer one.

    If there are holds for 15 days and 2 days, the actual hold will be 15 days.

### Example

Imagine that several actions happened on the account:

* registration → 15 days
* enabling Steam Guard → 7 days

➡️ both restrictions start at the same time, but the resulting hold is **15 days**

#### **Another example**

Imagine that you:

* disabled Steam Guard → 15 days
* 10 days passed
* enabled Steam Guard again → 7 days

➡️ Then from the moment of enabling, you will have 7 days:

* 5 days remaining from disabling Steam Guard
* 7 days from enabling Steam Guard

Both restrictions apply to trades and the market, so it will take 7 days from the moment of enabling Steam Guard until the restrictions are removed.

***

### 📋 Main types of holds

Below are the main actions that cause restrictions. Not all reasons are listed here, only the most common ones:

<table data-full-width="false"><thead><tr><th>Action</th><th>Duration</th><th>Scope</th></tr></thead><tbody><tr><td>Trade reversal, Trade-Protected</td><td>30 days</td><td>Trades + Market</td></tr><tr><td>Password reset, after 60+ days of inactivity</td><td>30 days</td><td>Trades + Market</td></tr><tr><td>Password reset</td><td>5 days</td><td>Trades + Market</td></tr><tr><td>Recovery through support, 60+ inactive</td><td>30 days</td><td>Trades + Market</td></tr><tr><td>Recovery through support</td><td>15 days</td><td>Trades + Market</td></tr><tr><td>Account registration</td><td>15 days</td><td>Trades + Market</td></tr><tr><td>Removing Steam Guard</td><td>15 days</td><td>Trades + Market</td></tr><tr><td>Enabling Steam Guard</td><td>7 days</td><td>Trades + Market</td></tr><tr><td>First purchase or top-up in a year</td><td>7 days</td><td>Market</td></tr><tr><td>Transferring mobile Steam Guard</td><td>2 days</td><td>Trades + Market</td></tr><tr><td>Changing nickname in Steam</td><td>2 <strong>hours</strong></td><td>Trades</td></tr></tbody></table>

***

### ✅ Summary

* all holds work **in parallel**
* final duration = **the longest active hold**
* short restrictions do not affect long ones

### ❓ Frequently asked questions

<details>

<summary><strong>Can changing the password impose restrictions?</strong></summary>

By itself, **changing the password** does not cause a hold. It is specifically a **password reset**, _Forgot password?_, if there has been no activity on your account for 60 days or more. Activity through the web version of Steam does not reset this period.

</details>

<details>

<summary><strong>If I traded with a person and they canceled the trade, will I also get a hold?</strong></summary>

No, the trade hold related to trade cancellations, Trade-Protected, is applied only to the account that initiates the cancellation. If you received a trade offer and canceled it, the hold will be only on you. If another person canceled the offer that you accepted, the hold will be only on them.

</details>

<details>

<summary><strong>Why can I still not trade even though 7 days have passed?</strong></summary>

Most likely, another longer hold is active on the account.

Check:

* whether the account was created recently
* whether Steam Guard was disabled
* whether a password reset was performed

Take into account not only the date, but also the time, restrictions are tied to the moment of the action and count exactly 24 hours, 7 days, and so on.

</details>