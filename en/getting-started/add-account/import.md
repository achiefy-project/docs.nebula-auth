---
icon: file-import
---

# Importing maFiles

Importing is the easiest way to add accounts to NebulaAuth. If you already have ready-made maFiles, for example from the old Steam Desktop Authenticator or another application, you can quickly transfer them into the application.

***

### Import methods

#### 1️⃣ Drag & Drop

The fastest option:

1. Open the folder with maFiles
2. Select the required files, or all at once
3. Drag them directly into the NebulaAuth window

The application will automatically recognize the format and add the accounts.

![Drag'n'Drop](../../../.gitbook/assets/drag-n-drop-demo.png)

***

#### 2️⃣ Paste from the clipboard (Ctrl + V)

A quick way for those who prefer the keyboard:

1. Select the files in Explorer
2. Press **Ctrl + C**
3. Go to the NebulaAuth window
4. Press **Ctrl + V**

All copied maFiles will be added automatically.

***

#### 3️⃣ Through the "File" menu

The classic way, suitable for adding a single file:

1. Click **File → Import**
2. Select the `.maFile` file
3. Click **Open**

![Mafile import in menu](../../../.gitbook/assets/menu-mafile-import.png)

### Additional information

#### 🔒 Encrypted maFile (migration from SDA)

NebulaAuth supports importing **encrypted maFiles** created in Steam Desktop Authenticator (SDA).

If your files are encrypted, during import the application will automatically prompt you to enter the **encryption password** that you used in SDA.

{% hint style="danger" %}
After a successful import, the maFiles will be saved **in decrypted form**.

In the current version of NebulaAuth, maFile encryption is not supported.
{% endhint %}

### How the import works

1. Start importing the maFile into NebulaAuth
2. When prompted, enter the encryption password from SDA
3. Wait for the import to complete

After that, the accounts will be added and ready to use.

### &#x20;Import completed, what's next?

After importing the accounts, it will appear in the list on the left.

In the following sections, you can learn about the main features of the application:

* [interface.md](../interface.md "mention") — the main interface elements and their purpose
* [first-steps.md](../first-steps.md "mention") — a quick start for receiving codes and confirming actions

### ❓ Frequently asked questions

<details>

<summary><strong>What should I do if the file already exists?</strong></summary>

If there is already a file with the same **name** in the `maFiles` folder, the application will offer you a choice of action:

* **Overwrite** — replace the existing file with the new one
* **Skip** — keep the existing file, do not add the new one

If several files are being imported, the selected action will be applied to all conflicts.

</details>

<details>

<summary><strong>Why is the maFile not being imported?</strong></summary>

Check the following:

* the file extension is **`.maFile`**
* the file opens in a text editor and contains **valid JSON**

Also make sure the file contains the required fields:

* `shared_secret`
* `identity_secret`
* `device_id`
* `account_name`

If these conditions are not met, the file will not be recognized as a valid maFile.

</details>

<details>

<summary><strong>Are maFiles compatible with Steam Desktop Authenticator (SDA)?</strong></summary>

Yes, maFiles are fully compatible.

Files from SDA can be imported into NebulaAuth and also used in other compatible applications.

</details>