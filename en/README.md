---
icon: galaxy
layout:
  width: default
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
  tags:
    visible: true
---

# Documentation

{% columns %}
{% column %}
NebulaAuth is an application that replaces the Steam mobile app\* when working with Steam Guard.

You can generate codes, confirm actions, and manage accounts from your computer without reaching for your phone.

<a href="getting-started/installation.md" class="button primary">Start setup</a>
{% endcolumn %}

{% column %}
<figure><img src="../.gitbook/assets/hero.png" alt=""><figcaption></figcaption></figure>
{% endcolumn %}
{% endcolumns %}

<sup>_<mark style="color:$info;">\*NebulaAuth is not an official Valve product and is not affiliated with Valve Corporation or Steam.</mark>_</sup>

## 🚀 Getting started

<table data-view="cards"><thead><tr><th></th><th></th><th data-hidden data-card-target data-type="content-ref"></th></tr></thead><tbody><tr><td>⚡ <strong>Quick start</strong></td><td>Install, launch, and add your first account</td><td><a href="getting-started/installation.md">installation.md</a></td></tr><tr><td>🔐 <strong>Linking and transfer</strong></td><td>Set up Steam Guard or transfer it from another device</td><td><a href="getting-started/add-account/">add-account</a></td></tr><tr><td><strong>❓Troubleshooting</strong></td><td>Fix common issues you may run into</td><td><a href="support/solving-problems.md">solving-problems.md</a></td></tr><tr><td>🤖 <strong>Automation</strong></td><td>Auto-confirmations and background operation</td><td><a href="features/auto-confirmations.md">auto-confirmations.md</a></td></tr><tr><td>🧾 <strong>maFile</strong></td><td>What it is and how to work with it</td><td><a href="steam-info/mafile/">mafile</a></td></tr><tr><td>⚙️ <strong>Settings</strong></td><td>Configure the application's behavior and appearance</td><td><a href="features/settings/">settings</a></td></tr></tbody></table>

***

### What NebulaAuth can do

NebulaAuth combines the main Steam Guard tasks in one place:

* creating/transferring Steam Guard on an account
* managing multiple accounts
* automatically confirming actions
* working with proxies

<details>

<summary>Rethinking SDA</summary>

NebulaAuth is inspired by Steam Desktop Authenticator (SDA) and builds on its ideas.

As workflows became more complex, the existing feature set was no longer enough. NebulaAuth adds broader functionality and a smoother approach to managing accounts.

</details>



### Security and control

NebulaAuth does not modify your account data or store it on external servers.

The project is open source, so you can review the code and verify how the application works.

All data remains with you:

* maFiles are stored locally
* passwords can be encrypted
* you fully control access

<details>

<summary>The application works locally and does not require third-party services</summary>

The application does not make third-party network requests, except to:

* Steam, to work with your account
* GitHub, to check for updates (optional during installation)

</details>



#### Official resources

For stable operation, security, and access to the latest updates, use only official and trusted sources.

* [💻 **Official repository**](https://github.com/achiez/NebulaAuth-Steam-Desktop-Authenticator-by-Achies/)
* [🚀 **Latest release**](https://github.com/achiez/NebulaAuth-Steam-Desktop-Authenticator-by-Achies/releases/latest)
* [📢 **Official Telegram channel (RU)**](https://t.me/nebulaauth)
* [**💬 Community chat**](https://t.me/nebulaauth_chat)
* [🧩 **.NET 8 Desktop Runtime**](https://dotnet.microsoft.com/en-us/download/dotnet/8.0)

***

#### Important

This documentation is the official NebulaAuth documentation.

It may be updated, reorganized, or moved to another domain without separate notice.\
We recommend using the project's GitHub repository as the primary and most up-to-date source for information and releases.
