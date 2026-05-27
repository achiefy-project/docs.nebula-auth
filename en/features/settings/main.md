# Main parameters

![Settings window](../../../.gitbook/assets/settings-main.png)

This section contains the main NebulaAuth settings that affect application behavior.

***

## Language

You can choose the interface language:

* English
* Русский
* Українська
* 简体中文
* Français
* Español
* Türkçe
* Қазақша

The language can be changed in the settings without restarting and without editing files.

***

## Hide to tray

When enabled, the application window is minimized to the system tray.

***

## Common maFile format

Enabled by default.

When enabled, NebulaAuth saves maFiles in a format compatible with Steam Desktop Authenticator, SDA.

When disabled, NebulaAuth uses its own format.

We do not recommend disabling this option, because many third-party tools expect the compatible format.

***

## Taskbar indicator

Adds a colored indicator to the application icon in the taskbar.

![Taskbar indicator](../../../.gitbook/assets/tray-color-indicator.png)

This is useful when working with multiple NebulaAuth windows, because it lets you quickly tell instances apart.

***

## Encryption password

Lets you set an encryption password for saved account passwords.

Enter the password and click **Save** to enable protection.

To remove the password, clear the field and save the changes.

More details: [Saving passwords](../session/saving-password.md)

***

## maFile names

Determines how file names are generated:

* by SteamID
* by account login

After changing this option, click **Apply**.

During the process:

* a backup copy of all maFiles is created in `maFiles_backup`
* the files are renamed
* the result is shown, including successes, conflicts, and errors
