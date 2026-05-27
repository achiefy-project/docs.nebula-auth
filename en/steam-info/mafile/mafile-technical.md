---
icon: code
---

# Technical information about the maFile

{% hint style="info" %}
This article is intended for advanced users.
{% endhint %}

***

### Basic Steam Guard fields

maFile is a JSON file containing Steam Guard data.

Main fields:

* `shared_secret`\
  Used to generate login codes, Steam Guard
* `identity_secret`\
  Used to confirm actions, trades, sales
* `revocation_code`\
  Code for removing Steam Guard from the account
* `account_name`\
  Steam account login
* `steamid`\
  Unique account identifier
* `device_id`\
  Generated device identifier. Used when working with confirmations.

***

### Additional Steam fields

The maFile may contain Steam service fields:

* `serial_number`
* `server_time`
* `token_gid`
* `secret_1`
* `uri`

These fields are either not used in operation, or their purpose is unknown.\
In NebulaAuth, they are not used and do not affect account operation.

***

### Session

The maFile may store the account session, authorization data.

NebulaAuth uses a modern session format, similar to the official Steam application:

* `access_token` — used to perform requests
* `refresh_token` — used to extend the session without logging in again

If `access_token` is outdated, NebulaAuth automatically tries to refresh it through `refresh_token`.

If this is not possible, for example the refresh token has expired, logging into the account again will be required.

{% hint style="info" %}
Steam Desktop Authenticator, SDA, uses an outdated format, an encoded session token.

Because of this, when importing a maFile from SDA, the session cannot be used, and you need to log into the account once.
{% endhint %}

### NebulaAuth fields

NebulaAuth adds its own fields:

* `Proxy`\
  Proxy assigned to the account
* `Group`\
  Account group
* `Password`\
  Saved password, in encrypted form

These fields are used only inside NebulaAuth and are not part of the Steam Guard format.

***

### ❓ Frequently asked questions

<details>

<summary><strong>Can I edit a maFile manually?</strong></summary>

Technically, yes.

But it is not recommended, an error in the file structure can make it unusable.

It is better to use NebulaAuth tools.

</details>

<details>

<summary><strong>Can I change the secrets, shared_secret, identity_secret?</strong></summary>

No.

These values are created by Steam when the authenticator is linked.

To get new ones, you need to remove Steam Guard and link it again.

</details>