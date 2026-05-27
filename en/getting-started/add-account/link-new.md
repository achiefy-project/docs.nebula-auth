---
icon: file-medical
---

# Linking an account

If mobile Steam Guard has never been enabled on your Steam account, or you have disabled it, you can link a new Steam Guard directly through **NebulaAuth**.

***

### ✅ Requirements

Before starting, make sure that:

* the account **does not have an active mobile Steam Guard**
* you have **access to the email** linked to the account
* you know the **login and password** of the Steam account

{% hint style="info" %}
**Trade hold**

After linking a new Steam Guard, your account will start a trade hold countdown of **7 days**. For new accounts, the delay will be up to **15 days**.

More details: [trade-hold.md](../../steam-info/trade-hold.md "mention")
{% endhint %}

### 🧭 Linking process

![Linker View](../../.gitbook/assets/linker-view.png)

#### Step 1: Launch the linking wizard

1. In the top menu, click **Account → Link**
2. The linking wizard window will open

***

#### Step 2: Log into the account

Enter the login details:

* **Login** — the name of the Steam account
* **Password** — the password for the account
* **Proxy** (optional) — the selected proxy will be used during the linking process

Click **Continue**.

***

#### Step 3: Code from email, if email Guard is enabled

If email Steam Guard is enabled on the account, a confirmation code will be sent to your email.

1. Enter the code
2. Click **Continue**

If email Guard was not enabled, this step is skipped automatically.

***

#### Step 4: Phone number, optional

Steam may ask you to enter a phone number. At the moment, **this is not required**.

Possible options:

* **Enter a phone number** → SMS confirmation will be required
* **Skip the step** → the confirmation code will be sent by email

***

#### Step 5: Confirmation

The next actions depend on the previous step:

* if you entered a phone number, enter the **SMS code**
* if the number was skipped, enter the **code from email**

If the phone number **had already been linked to the account before**, the confirmation code always arrives **by SMS**, even if the phone number step was skipped.

***

#### Step 6: Done

Linking is complete. The screen will display:

* **R-code (Revocation Code)** Write it down and store it in a safe place _(best of all on paper)_
* **File name** — under this name the maFile is saved in the `maFiles` folder

{% hint style="info" %}
NebulaAuth automatically creates a backup of the maFile in the `maFiles_backup` folder. This is additional protection in case the main file is lost or the linking process fails
{% endhint %}

The maFile is automatically added to the account list. Now you can receive Guard codes and, after the temporary trade ban, begin confirming item actions.

### ⚠️ What should I do if an error occurs?

Sometimes the linking process may end with an error. The most common messages are:

* `BadConfirmationCode`
* `InvalidState`
* "The code did not fit"

This is a **known bug on Steam's side** and is not an error of our application.

***

### 🔧 Solution

_Follow the steps exactly_

If the error appears, perform the steps **strictly in order**:

1. **Start the linking process again**
2. Enter the login and password
3. When asked for a phone number, enter any real phone number
4. Follow the link from the email
5. Click **Continue**

Then two scenarios are possible:

**Scenario A: An error appeared** If any error appears, proceed to step 6

**Scenario B: SMS code request** If the system requests an SMS:

* ❗ **Do not enter the SMS code**
* Close the linking window
* Wait 20 minutes for Steam to reset the state

6. After that, the problem should disappear
7. Repeat the linking process in the normal way

{% hint style="warning" %}
After **3-5 failed attempts**, Steam may block linking for a period from **1 day to a week**.

If an error appears, **do not continue blindly**, use the instructions above immediately.
{% endhint %}

***

#### Why does this work?

This is a known peculiarity in Steam logic. When you go through the process with a phone number, Steam removes the internal "lock", and subsequent linking becomes possible.

### ✅ Linking completed, what's next?

After linking, the account will appear in the list on the left.

In the following sections, you can learn about the main features of the application:

* [interface.md](../interface.md "mention") — the main interface elements and their purpose
* [first-steps.md](../first-steps.md "mention") — a quick start for receiving codes and confirming actions

### ❓ Frequently asked questions

<details>

<summary><strong>Can I link an account if Steam Guard is already enabled on another device?</strong></summary>

No.

If mobile Steam Guard is already active, use [**Steam Guard transfer**](transfer.md).

If you want to link Guard again:

1. Disable the current Steam Guard
2. Wait until the cooldown ends, **15 days**
3. After that, perform the linking through NebulaAuth

</details>

<details>

<summary><strong>Why is an SMS code requested if I did not enter a phone number?</strong></summary>

Possible reasons:

* the phone number is already linked to the account
* the number was entered earlier, Steam may remember it for **20-30 minutes**

In that case:

* wait some time
* repeat the linking process

</details>

<details>

<summary><strong>I get a LimitExceeded error or other errors after several attempts</strong></summary>

Steam limits the number of linking attempts.

After several failed attempts, a temporary block may be set:

* from **24 hours** to **several days**

It is recommended to:

* stop trying
* wait
* then repeat the process, strictly following the instructions above

</details>

<details>

<summary><strong>I followed the bug fix instructions, but the error still appears</strong></summary>

Some accounts may be more sensitive to this Steam behavior.

In this case, it is recommended to:

1. Go to the official Steam website through a browser
2. Link the phone number manually
3. After that, return to NebulaAuth and finish linking via SMS

</details>