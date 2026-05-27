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

You can receive codes, confirm actions, and manage accounts without a phone, faster and more conveniently.

<a href="getting-started/installation.md" class="button primary">Start setup</a>
{% endcolumn %}

{% column %}
<figure><img src=".gitbook/assets/hero.png" alt=""><figcaption></figcaption></figure>
{% endcolumn %}
{% endcolumns %}

<sup>_<mark style="color:$info;">\*NebulaAuth is not an official Valve product and is not affiliated with Valve Corporation or Steam.</mark>_</sup>

## 🚀 Getting started

<table data-view="cards"><thead><tr><th></th><th></th><th data-hidden data-card-target data-type="content-ref"></th></tr></thead><tbody><tr><td>⚡ <strong>Quick start</strong></td><td>Installation, launch, and adding your first account</td><td><a href="getting-started/installation.md">installation.md</a></td></tr><tr><td>🔐 <strong>Linking and transfer</strong></td><td>Connecting Steam Guard or transferring it from another device</td><td><a href="getting-started/add-account/">add-account</a></td></tr><tr><td><strong>❓Troubleshooting</strong></td><td>Solving common issues that arise during use</td><td><a href="support/solving-problems.md">solving-problems.md</a></td></tr><tr><td>🤖 <strong>Automation</strong></td><td>Auto-confirmations and background operation</td><td><a href="features/auto-confirmations.md">auto-confirmations.md</a></td></tr><tr><td>🧾 <strong>maFile</strong></td><td>What it is and how to work with it</td><td><a href="steam-info/mafile/">mafile</a></td></tr><tr><td>⚙️ <strong>Settings</strong></td><td>Configuring the application's behavior and appearance</td><td><a href="features/settings/">settings</a></td></tr></tbody></table>

***

### What NebulaAuth can do

NebulaAuth combines the main Steam Guard tasks in one place:

* creating/transferring Steam Guard on an account
* managing multiple accounts
* automatically confirming actions
* working with proxies

<details>

<summary>Rethinking SDA</summary>

NebulaAuth is inspired by Steam Desktop Authenticator (SDA) and develops its ideas further.

During development, it became clear that the existing capabilities were not enough for more complex workflows, so NebulaAuth offers expanded functionality and a more convenient approach to account management.

</details>



### Security and control

NebulaAuth does not modify account data and does not store information on external servers.

This is an open-source project, you can review the code and verify how the application works.

All data remains with you:

* maFile is stored locally
* passwords can be encrypted
* you fully control access

<details>

<summary>The application works locally and does not require third-party services</summary>

The application does not perform third-party network requests, except:

* Steam, for working with the account
* GitHub, for checking updates (installation optional)

</details>



#### Official resources

To ensure stable operation, security, and access to up-to-date updates, it is recommended to use only official and trusted sources.

* [💻 **Official repository**](https://github.com/achiez/NebulaAuth-Steam-Desktop-Authenticator-by-Achies/)
* [🚀 **Latest release**](https://github.com/achiez/NebulaAuth-Steam-Desktop-Authenticator-by-Achies/releases/latest)
* [📢 **Official Telegram channel (RU)**](https://t.me/nebulaauth)
* [**💬 Community chat**](https://t.me/nebulaauth_chat)
* [🧩 **.NET 8 Desktop Runtime**](https://dotnet.microsoft.com/en-us/download/dotnet/8.0)

***

#### Important

This documentation is the official NebulaAuth documentation.

At the same time, it may be updated, change structure, or be moved to another domain without separate notice.\
It is recommended to use the project's GitHub repository as the main and most up-to-date source of information and updates.