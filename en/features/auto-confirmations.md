---
icon: robot
---

# Auto-confirmations

![MAAC](../../.gitbook/assets/mw-maac.png)

Auto-confirmations let NebulaAuth automatically confirm actions in Steam without manually opening each account.

This is convenient if you work with several accounts and want to process sales or trades faster.

***

### What can be confirmed

For each account, you can enable separately:

* **purchases and sales on the Market**
* **trades**

These modes are independent of each other. For example, you can enable only sales confirmation, only trade confirmation, or both options at once.

{% hint style="warning" %}
At the moment, NebulaAuth does not accept trades automatically.

The application can only confirm already created or accepted trades.
{% endhint %}

***

### Where auto-confirmations are enabled

Auto-confirmations can be enabled:

* for one selected account
* for the selected group of accounts
* for all accounts at once

This lets you quickly configure the operating mode both for a separate account and for a large list.

After restart, all settings are saved, and you do not need to enable auto-confirmations again.

***

### How it works

After this function is enabled, NebulaAuth periodically checks accounts for actions that require confirmation.

If a confirmation is found, the application will perform it automatically according to the selected settings.

The check interval is set in the upper part of the window next to the auto-confirmation switches

{% hint style="info" %}
It is not recommended to set too small an interval for a large number of accounts.\
If there are many accounts, it is better to increase the check interval or use different proxies to reduce the number of requests to Steam from one IP address.
{% endhint %}

***

### Errors and statuses

If errors occur during checking, NebulaAuth displays the account state in the interface, the color changes.

The behavior is as follows:

* first the account becomes **yellow**, this means a temporary problem
* if the error persists and the account cannot recover, it becomes **red**

Usually problems are related to:

* unstable proxy
* outdated session
* maintenance on Steam's side, for example Tuesday-Wednesday

If the account stays in an error state for a long time, you can:

* log into the account again
* restart the timer for this account

This will reset the state and start a repeated check.

***

### After restarting the application

Confirmation settings are saved after restarting NebulaAuth.

All settings are preserved, and the application will continue working in the same mode as before closing.

***

### Recommendations

* use stable proxies
* do not set too small a check interval
* increase the interval for a large number of accounts
* if errors appear, first check the proxy and the account session