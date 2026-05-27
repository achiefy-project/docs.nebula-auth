---
icon: window
---

# Interface overview

After launching NebulaAuth, you will see the main application window. It is divided into several logical parts, each responsible for its own task. Below we will go through them in order.

![NebulaAuth main window](../.gitbook/assets/main-window.png)

***

## 🧭 Control panel, top section

At the top of the window there is a panel with the menu and controls.

![Control panel](../.gitbook/assets/interface-control-panel.png)

### Menu

The main actions related to maFiles and application settings are collected here:

* **Import** — add maFiles to the application
* **Delete** — delete the selected maFile from NebulaAuth
* **Open folder** — open the folder where maFiles are stored
* **Proxy manager** — open proxy management
* **Settings** — change the language, appearance, and behavior of the application

Additional functions are available in the **"Other"** subsection:

* **Set passwords** — set passwords for several accounts at once
* **Export** — save maFiles to another folder or with the required parameters

***

### "Account" menu

This menu is responsible for actions with Steam accounts:

* **Link** — create a new Steam Guard for the account
* **Transfer Steam Guard** — transfer Guard from the phone to the computer
* **Remove** — completely remove Steam Guard from the account
* **Refresh session** — try to refresh the account session without a password
* **Login again** — log into the account again if the session is outdated

***

### Groups

A field for selecting or creating account groups.

If you have many accounts, you can combine them into groups, for example: "Main", "Farm", "Trade".

* When a group is selected, only accounts from it are displayed in the list
* To create a new group, enter its name and press **Enter**

More details: [groups.md](../features/groups.md "mention")

***

### Proxy

Here the proxy associated with the current account is selected and displayed. To assign a proxy, you first need to create it in the **Proxy manager**, the button is in the menu. After creation, it will appear in this list.

An indicator may be displayed next to the field:

* **Yellow circle** — the default proxy is used
* **Red circle** — the proxy is specified in the maFile, but is missing in the application

When you hover over the indicator, a tooltip with detailed information will appear.

More details: [proxy](../features/proxy/ "mention")

***

### Auto-confirmation timers

Two switches are responsible for automatic confirmations:

* **"Cart"** — confirmation of sales and purchases on the Steam Community Market
* **"Person with arrow"** — confirmation of trades

Next to it there is a field with the check interval, in seconds. The application will check for new confirmations at the specified frequency.

> By right-clicking the switches, you can enable timers for the entire group of accounts or for all accounts at once.

More details: [auto-confirmations.md](../features/auto-confirmations.md "mention")

***

### Show accounts with auto-confirmation

The button with the **Accounts** icon on the right.

If enabled, only those accounts that have auto-confirmations active are displayed in the account list.

***

## 👥 Account list, left section

The left side of the window shows all added accounts. Each account is shown under its login

![Account list](../.gitbook/assets/interface-account-list.png)

At the bottom of the list there is a search field. You can search for accounts by login or SteamID, which starts with `76...`.

***

### Account context menu

Right-clicking an account opens a menu:

* Copy login
* Copy password
* Copy SteamID
* Copy maFile
* Add to group
* Remove from group
* Unbind proxy

***

## 🔐 Codes and confirmations, right section

The right side of the window lets you interact with the selected account.

![Codes and confirmations](../.gitbook/assets/interface-codes-and-confirmations.png)

***

### Confirmation code

The current Guard code is displayed at the top. Click it to copy it.

Under the code there is a time indicator showing how many seconds remain until the update. The code changes every 30 seconds.

***

### Load confirmations

Button for receiving confirmations from Steam servers.

> Confirmations appear **only after an action** that requires them, for example a trade, sale, and so on.

After loading, confirmation cards will appear below, which can be accepted or rejected.

***

### Confirm login

Button in the lower part of the panel.

Used to confirm a login to Steam from a new device:

* if there is **one** request, the login is confirmed immediately
* if there are **multiple** requests, the button does nothing

In this case, it is recommended to confirm the login manually through the confirmation list.

***

## ℹ️ Bottom panel

At the bottom of the window service information is displayed:

* the number of loaded accounts
* the name of the selected account
* the **by achies** link, the official source and author of the project

***

## What's next?

Now that you are familiar with the interface, you can move on to studying the main functions of the application.

To start working with accounts, we recommend reading the sections:

{% content-ref url="first-steps.md" %}
[first-steps.md](first-steps.md)
{% endcontent-ref %}

{% content-ref url="../features/proxy/" %}
[proxy](../features/proxy/)
{% endcontent-ref %}