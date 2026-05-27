---
icon: users
---

# Adding accounts

This section introduces you to the different ways of adding accounts to NebulaAuth. You can learn more about each method by following the corresponding links.

### 🧭 Which method should you choose?

The application supports three main ways of adding accounts, each suitable for different situations

<details>

<summary><strong>✅ Method 1: Import ready-made maFiles</strong></summary>

Suitable if you already have maFiles (`.maFile`), for example from Steam Desktop Authenticator or another source.

You can import maFiles in any convenient way:

* **Drag & Drop** Just drag the `.maFile` files directly into the NebulaAuth window.
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

Suitable if **Steam Guard is not yet enabled** on the account.

1. Click **Account → Link**
2. Follow the linking wizard instructions

After linking, the standard Steam trade restriction of **7-15 days** applies.

More details: [link-new.md](link-new.md "mention")

</details>

<details>

<summary><strong>📱 Method 3: Transfer Steam Guard from the phone (2 days trade ban)</strong></summary>

Suitable if Steam Guard is already active on a mobile device.

1. Click **Account → Transfer Steam Guard**
2. Follow the transfer wizard instructions

After the transfer, a **2-day** trade delay usually applies.

More details: [transfer.md](transfer.md "mention")

</details>

### 📁 Where are maFiles stored?

All imported maFiles are saved in the `maFiles` folder, which is located next to the **NebulaAuth.exe** file.

To quickly open this folder:

* click **File → Open folder**

### 📄 What happens when you add an account?

With any method of adding, a `maFiles` folder is created next to the application. It stores a maFile, a file with the `.maFile` extension.

This file contains **all information** for:

* generating Guard codes
* confirming trades
* confirming logins

{% hint style="warning" %}
The maFile is the most important file for Steam Guard. Without it, restoring two-factor authentication will be impossible.
{% endhint %}

We recommend:

* making backups of the `maFiles` folder
* never deleting or modifying these files manually
* storing the R-Code in a safe place, best of all on **paper**, not in digital form

After adding accounts, NebulaAuth is ready to use. If your workflow involves using proxies, do not forget to configure them before you start interacting with accounts (_more details in the_ [proxy](../../features/proxy/ "mention") _section_).

In the following sections, you can learn about the main features of the application:

* [interface.md](../interface.md "mention") — the main interface elements and their purpose
* [first-steps.md](../first-steps.md "mention") — a quick start for receiving codes and confirming actions

### ❓ Frequently asked questions

<details>

<summary><strong>Can I use one account in multiple applications at the same time?</strong></summary>

Yes, it is possible if you have a **maFile**.

The file can be used on multiple devices or in different applications at the same time, it contains all the necessary data.

If Steam Guard is linked to the mobile application, it is impossible to obtain the **maFile** directly without interfering with the device system.

</details>