---
icon: file-lines
---

# What is a maFile

**maFile** is a file that stores access to your account's Steam Guard.

It is needed for:

* generating login codes
* confirming trades and sales
* managing the authenticator

***

### How NebulaAuth works with maFile

When started, NebulaAuth automatically reads all maFiles from the `maFiles` folder.

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
Anyone who has access to the maFile can use your Steam Guard.

Do not share these files with outsiders.
{% endhint %}

It is recommended to:

* store maFile in a safe place
* make backup copies
* save the RCode, recovery code, separately

***

### More details

In the next section, you can learn about the technical information on the maFile structure

{% content-ref url="mafile-technical.md" %}
[mafile-technical.md](mafile-technical.md)
{% endcontent-ref %}