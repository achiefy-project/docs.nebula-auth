---
hidden: true
---

# Advanced settings (WIP)

This section contains parameters that directly affect proxies and auto-confirmations.

## Proxy display settings

Parameters:

* `ProxyManagerDisplayProtocol`
* `ProxyManagerDisplayCredentials`

They control only the display in the proxy manager and do not change the network logic itself.

## Auto-confirmation parameters

### TimerSeconds

* the main timer interval in seconds
* minimum value in the UI: 5 seconds

### MaacErrorThreshold

* after how much time of continuous errors the account is moved to the error status
* default: 3 hours

### MaacRetryInterval

* retry interval after an error in warning state
* default: 15 minutes

## How error logic is applied

MAAC uses statuses:

* `Ok` — everything works
* `Warning` — there is an error, but retries will occur through `MaacRetryInterval`
* `Error` — the error lasts longer than `MaacErrorThreshold`

When the problem disappears, the status returns to `Ok`.

Select an account in the list and look at the auto-confirmation indicator in the right panel:

* **Green** — OK
* **Yellow** — Warning
* **Red** — Error

**Do MAAC settings affect manual confirmations?**

No, MAAC settings affect only **automatic** confirmations. Manual confirmations, through the "Load confirmations" button, work independently.

**Can I configure different intervals for different accounts?**

No, the timer interval is shared for all accounts. However, you can run **multiple copies of NebulaAuth** with different settings for different account groups.

***

## Related sections

* [Main settings](main.md)
* [Appearance](appearance.md)
* [Security](/broken/pages/bDMQ398cvxmpLYhOiFUF)
* [Auto-confirmations](../auto-confirmations.md)
* [Proxy](../proxy/)