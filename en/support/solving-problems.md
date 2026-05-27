---
icon: lightbulb-exclamation-on
---

# Troubleshooting

Typical errors and ways to solve them are listed below.

***

### Connection errors

* **"An existing connection was forcibly closed by the remote host"**
* **"No connection could be made because the target machine actively refused it"**

Usually related to:

* proxy problems
* unstable internet connection

Solution:

* check the proxy
* try another proxy
* make sure the internet works stably

***

### Response ended prematurely

If the error occurs constantly:

* most likely a SOCKS proxy is used without specifying the protocol\
  for example specify: `socks5://IP:PORT`

If it occurs occasionally:

* these are temporary connection drops on Steam's side

***

### Accounts disappeared, RCode, password do not work

If you downloaded NebulaAuth from the official source:

* the application does not modify account data
* the problem is on the user side

It is recommended to contact Steam Support.

***

### Steam Guard code does not fit

Reason:

* time desynchronization on the PC

Solution:

* synchronize the time with the internet
* restart the application

***

### Error when linking: BadConfirmationCode

This is a known Steam issue.

Solution:

* use the instructions at the top of the linking window
* or see the section: [Linking → Problem solution](../getting-started/add-account/link-new.md#-solution)

***

### "Failed to synchronize time with Steam"

An error that occurs when the application starts

Reasons:

* maintenance work on Steam's side
* connection problems

Solution:

* check the internet
* try disabling or changing the VPN

***

### Session fully expired

Solution:

1. Select the account
2. Click **Account → Login**
3. Enter the password