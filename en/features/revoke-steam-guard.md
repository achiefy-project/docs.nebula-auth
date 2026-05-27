---
icon: user-minus
---

# Removing Steam Guard

![Confirmation of removal](../../.gitbook/assets/confirm-revoke.png)

Removing Steam Guard deletes the mobile authenticator from the account.

After the operation completes, Steam Guard stops working and a trade hold is applied to the account.

***

### Before you start

Removal requires a **revocation code (RCode)**.

It is automatically stored in the **maFile** when linking or transferring Steam Guard.

If the RCode is missing, NebulaAuth cannot remove Steam Guard.

***

### How to remove Steam Guard

1. Select the account
2. Click **Account → Remove**
3. Confirm the action

If the operation succeeds:

* Steam Guard will be removed
* a **15-day** hold is applied to trades and the Market
* the maFile will be moved to the `maFiles_removed` folder

More details: [Trade hold](../steam-info/trade-hold.md)

***

### If it did not work

Try:

* checking the account session
* using **Login Again**
* trying the removal again

If the maFile is lost or the RCode in it is invalid, contact Steam Support to restore access to the account.

***

### Deleting an account, maFile

Deleting an account in NebulaAuth is a separate action.

When deleting:

* the maFile is moved to the `maFiles_removed` folder
* the account disappears from the list

**Important**

This **does not remove Steam Guard**.

If Steam Guard is still linked, you can restore the account in NebulaAuth by importing the maFile again.

***

### How to delete an account

1. Select the account
2. Menu → **Delete**
3. Confirm the action

***

### ❓ Frequently asked questions

<details>

<summary><strong>Why is the "Remove" button unavailable?</strong></summary>

The button becomes active only if `revocation_code` is present in the selected maFile.

</details>

<details>

<summary><strong>Can I remove Steam Guard if there is no password and the session has expired?</strong></summary>

No.

An active account session is required to remove Steam Guard through NebulaAuth.

If there is no session, use the RCode through "Forgot password" on the Steam website or contact support.

</details>

<details>

<summary><strong>What should I do if both the maFile and the RCode are lost?</strong></summary>

Contact Steam Support.

To restore access, you will need to prove account ownership using purchases, payments, and other account details.

</details>

<details>

<summary><strong>Can I remove Steam Guard if the account is blocked?</strong></summary>

It depends on the type of block.

* with a trade ban or VAC ban, yes
* with a red table warning, no, because account data cannot be changed.

</details>
