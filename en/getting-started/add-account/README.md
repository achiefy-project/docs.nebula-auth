---
icon: users
---

# Adding accounts

This section explains the different ways to add accounts to NebulaAuth. Each method has its own detailed page.

### 🧭 Which method should you choose?

The application supports three main ways to add accounts. Each one is useful in a different situation.

<details>

<summary><strong>✅ Method 1: Import ready-made maFiles</strong></summary>

Use this if you already have maFiles (`.maFile`), for example from Steam Desktop Authenticator or another source.

You can import maFiles in whichever way is most convenient:

* **Drag & Drop** Drag the `.maFile` files directly into the NebulaAuth window.
* **From the clipboard**
  1. Select the maFiles in Explorer
  2. Press **Ctrl + C**
  3. Go to the NebulaAuth window
  4. Press **Ctrl + V**
* **Through the menu**
  1. Click **File → Import**
  2. Select the `.maFile` on your computer
  3. Click **Open**

More details: [import.md](import.md "mention")

</details>

<details>

<summary><strong>🔗 Method 2: Link a new account</strong></summary>

Use this if **Steam Guard is not enabled yet** on the account.

1. Click **Account → Link**
2. Follow the linking wizard instructions

After linking, the standard Steam trade restriction of **7-15 days** applies.

More details: [link-new.md](link-new.md "mention")

</details>

<details>

<summary><strong>📱 Method 3: Transfer Steam Guard from the phone (2 days trade ban)</strong></summary>

Use this if Steam Guard is already active on a mobile device.

1. Click **Account → Transfer Steam Guard**
2. Follow the transfer wizard instructions

After the transfer, a **2-day** trade delay usually applies.

More details: [transfer.md](transfer.md "mention")

</details>

### 📁 Where are maFiles stored?

All imported maFiles are saved in the `maFiles` folder next to **NebulaAuth.exe**.

To quickly open this folder:

* click **File → Open folder**

### 📄 What happens when you add an account?

Whichever method you use, NebulaAuth creates a `maFiles` folder next to the application. This folder stores maFiles, which are files with the `.maFile` extension.

Each file contains **all information** needed for:

* generating Guard codes
* confirming trades
* confirming logins

{% hint style="warning" %}
The maFile is the most important Steam Guard file. Without it, you will not be able to restore two-factor authentication through NebulaAuth.
{% endhint %}

We recommend:

* making backups of the `maFiles` folder
* never deleting or modifying these files manually
* storing the R-Code in a safe place, preferably on **paper** rather than digitally

After adding accounts, NebulaAuth is ready to use. If your workflow uses proxies, configure them before working with accounts (_more details in the_ [proxy](../../features/proxy/ "mention") _section_).

The following sections cover the main application features:

* [interface.md](../interface.md "mention") — the main interface elements and their purpose
* [first-steps.md](../first-steps.md "mention") — a quick start for generating codes and confirming actions

### ❓ Frequently asked questions

<details>

<summary><strong>Can I use one account in multiple applications at the same time?</strong></summary>

Yes, if you have a **maFile**.

The file can be used on multiple devices or in different applications at the same time because it contains all required data.

If Steam Guard is linked only to the mobile app, you cannot obtain the **maFile** directly without accessing the device system.

</details>
