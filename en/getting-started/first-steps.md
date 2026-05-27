---
icon: shoe-prints
---

# First steps

This section is intended to introduce the main functions of NebulaAuth. Here you will learn how to receive login codes, as well as confirm trades and logins on other devices.

## 🔐 Getting a login code

Logging in with a Steam Guard code is the standard two-factor authentication in Steam. The code is generated based on the secrets stored in the maFile and updates every 30 seconds.

![Steam Guard code](../../.gitbook/assets/steam-guard-code.png)

{% hint style="info" %}
An internet connection is not required to generate codes
{% endhint %}

Getting a code:

1. Select the account in the list on the left
2. The Guard code will be displayed on the right side of the window
3. Click the code to copy it

The code updates every 30 seconds. The indicator under the code shows the time until the next update.

***

### 🔁 Confirming trades and sales

Confirmations appear **only after an action** that requires them, for example selling an item on the market or sending a trade.

1. Perform the action in Steam, trade, sale, and so on
2. Select the account in NebulaAuth
3. Click **Load confirmations**
4. Confirmation cards will appear below
5. Click ✔️ (**Confirm**) or ✖️ (**Reject**)

![alt text](../../.gitbook/assets/confirmations.png)

## 📱 Confirming login on another device

If you are logging into Steam from a new computer or browser:

1. Enter your login and password in Steam
2. Open NebulaAuth
3. Select the account
4. Click **Confirm login**
5. Return to the browser or Steam application, authentication will be completed

{% hint style="info" %}
The **"Confirm login"** button only works for one login at a time. If multiple login attempts are detected, the request will be rejected. This does not necessarily mean someone is trying to hack your account, most likely there were several login attempts in a short period of time.
{% endhint %}

## 🚀 What's next?

Now you know the basics of working with NebulaAuth.

We recommend studying further:

* [proxy](../features/proxy/ "mention")
* [auto-confirmations.md](../features/auto-confirmations.md "mention")
* [groups.md](../features/groups.md "mention")
* [settings](../features/settings/ "mention")

If you have questions, take a look at the [solving-problems.md](../support/solving-problems.md "mention") section or ask them in our [Telegram community](https://t.me/nebulaauth_chat).