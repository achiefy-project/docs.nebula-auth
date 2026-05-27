---
icon: key
---

# Working with the session

The session is the logged-in state of a Steam account.

It is stored inside the **maFile** and lets NebulaAuth perform actions without asking for the password again.

***

### How it works

After login, NebulaAuth saves the mobile session of the account.

It usually stays valid for a long time, often up to several months, so you do not need to enter the password every time.

However, the session can be reset:

* when the IP address changes
* when the password changes
* for internal Steam reasons

***

### If the session has expired

If a session error appears, log in again:

1. Select the account
2. Click **Account → Login**
3. Enter the password

After that, the session will be updated and saved in the maFile.

***

### Automatic login

You can enable password saving.

In that case, NebulaAuth can restore the session automatically without your involvement.

The password is stored in encrypted form.

More details: [saving-password.md](saving-password.md "mention")

***

### After transfer from SDA

After importing a maFile from Steam Desktop Authenticator, all accounts will show **"Session fully expired"**.

This is normal.

After the import, you need to **log in once** for each account.

***

### "Refresh session" button

Steam uses two types of sessions:

* long-lived, main
* short-lived, working

The **"Refresh session"** button refreshes the short session if possible.

{% hint style="info" %}
In newer versions of NebulaAuth, this is usually not required because the application tries to restore the session automatically.
{% endhint %}

***

### ❓ Frequently asked questions

<details>

<summary><strong>What happens if I change the Steam password?</strong></summary>

All active sessions will be reset.

After that, you need to log into NebulaAuth again.

</details>

<details>

<summary><strong>What does the "Refresh session" button do?</strong></summary>

Steam uses two types of sessions:

long-lived, main; short-lived, working

The "Refresh session" button tries to refresh the short session without re-entering the password.

{% hint style="info" %}
In most cases, you do not need to use this button because NebulaAuth automatically tries to restore the session.

If an error occurs, it is easier to use Account → Login.
{% endhint %}

</details>
