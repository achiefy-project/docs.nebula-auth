---
icon: file-lines
---

# What is a maFile

A **maFile** is a file that stores the data needed to use your account's Steam Guard.

It is needed for:

* generating login codes
* confirming trades and sales
* managing the authenticator

***

### How NebulaAuth works with maFiles

When it starts, NebulaAuth automatically reads all maFiles from the `maFiles` folder.

After that, they are displayed in the **"Accounts"** section inside the interface.

{% hint style="info" %}
Unlike Steam Desktop Authenticator, SDA, NebulaAuth does not require the `manifest.json` file.
{% endhint %}

***

### Where the files are located

NebulaAuth uses several folders:

* `maFiles` — working accounts
* `maFiles_removed` — deleted accounts
* `maFiles_backup` — backup copies

***

### Security

{% hint style="danger" %}
Anyone with access to a maFile can use your Steam Guard.

Do not share these files with outsiders.
{% endhint %}

It is recommended to:

* store maFiles in a safe place
* make backup copies
* save the RCode, recovery code, separately

***

### More details

The next section covers technical information about the maFile structure.

{% content-ref url="mafile-technical.md" %}
[mafile-technical.md](mafile-technical.md)
{% endcontent-ref %}
