---
icon: file-export
---

# Exporting maFiles

In NebulaAuth, you can quickly export a maFile to the required folder by specifying the account list and selecting the necessary parameters.

This is useful when you need to transfer accounts to another instance of the application, make a backup, or prepare files for use in other tools.

To avoid configuring export again every time, NebulaAuth uses templates.

![Export window](../../.gitbook/assets/mafile-export.png)

***

### What is a template

A template is a preset that defines:

* which fields to include in the export
* where to save the files
* how to form file names

You can create and save templates with your own names for convenience.

***

### How to perform export

1. Open **Menu → Other → Export**
2. Select the template or required fields
3. Specify the account list, logins or SteamID, one per line
4. Select the destination folder
5. Start the export
6. The found accounts will be copied to the selected folder

***

### Field configuration

When configuring the template, you can choose which data to include in the maFile:

* main fields, `shared_secret`, `identity_secret`, `revocation_code`
* session data
* additional maFile fields
* NebulaAuth fields, `Proxy`, `Group`, `Password`
* file name format, by SteamID or by login

To learn what exactly is exported and why this field is needed, hover over the field and wait for the tooltip.

More details: [mafile-technical.md](../steam-info/mafile/mafile-technical.md "mention")

***

#### Restrictions

* export to NebulaAuth folders, `maFiles`, `maFiles_removed`, `maFiles_backup`, is prohibited
* if a file with the same name already exists, it will NOT be overwritten
* exported files without the main fields will not work in NebulaAuth, because it requires all main data to be present for correct operation

***

### Partial export, truncated maFile

Sometimes a so-called **truncated maFile** is used.

This is a file that contains only:

* the account login
* `shared_secret`

Such a maFile:

* lets you generate login codes
* **does not give access to confirmations and Steam Guard**

{% hint style="danger" %}
**Even a truncated maFile is not completely safe.**

Do not pass such files to people you do not trust.\
They can be used for unwanted activity, for example login to the account, spam, or other actions.
{% endhint %}

***

### Export result

After completion, you receive a report:

* how many accounts were exported
* how many were not found
* how many conflicts occurred