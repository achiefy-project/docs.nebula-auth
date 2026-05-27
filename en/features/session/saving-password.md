---
icon: lock
---

# Saving passwords

NebulaAuth lets you save account passwords so it can restore sessions automatically without your involvement. This feature also lets you quickly copy a password from the account context menu; see [Context menu](../../getting-started/interface.md#account-context-menu).

***

### How it works

When necessary, for example if the session has expired, the application can log into the account again.

The saved password is used for this.

If password saving is enabled:

* it is written to the **maFile**
* it is used for automatic login
* it does not require manual input when the session fails

***

### Password protection

Passwords are not stored in plain text.

An **encryption password**, set in NebulaAuth, is used to protect them. See [Security settings](../settings/main.md#encryption-password)

* the account password is stored in encrypted form
* the encryption password is not stored on disk
* after restart, it must be entered again

If you forget the encryption password, saved passwords cannot be restored. This does not affect the accounts themselves, but automatic login will stop working, and you will need to assign passwords again for each account.

***

### What is important to understand

* only the account password is encrypted, not the whole maFile
* without the encryption password, automatic login will not work
* when transferring a maFile, the encrypted password is transferred with it

***

### Mass password assignment

You can save passwords for several accounts at once.

#### Format

Each line corresponds to one account:

```id="mass-pass"
login:password
SteamID:password
```

***

#### How to use

1. Open Menu → Other → Set passwords
2. Enter the encryption password if it is not set yet
3. Paste the list of lines
4. Confirm the changes

The format must be one of the following:

* `login:password`
* `SteamID:password`

After applying the changes, you will see how many passwords were assigned successfully.

## ❓ Frequently asked questions

<details>

<summary><strong>How do I remove the password prompt on startup?</strong></summary>

Clear the encryption password field in the settings and save the changes.

After that, NebulaAuth will not ask for a password on startup.

See [Settings → Encryption password](../settings/main.md#encryption-password)

</details>
