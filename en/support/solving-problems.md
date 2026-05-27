---
icon: lightbulb-exclamation-on
---

# Troubleshooting

Common errors and ways to fix them are listed below.

***

### Connection errors

* **"An existing connection was forcibly closed by the remote host"**
* **"No connection could be made because the target machine actively refused it"**

Usually caused by:

* proxy problems
* unstable internet connection

Solution:

* check the proxy
* try another proxy
* make sure your internet connection is stable

***

### Response ended prematurely

If the error happens constantly:

* most likely, a SOCKS proxy is being used without specifying the protocol\
  for example, use: `socks5://IP:PORT`

If it occurs occasionally:

* it is likely caused by temporary connection drops on Steam's side

***

### Accounts disappeared, RCode or password does not work

If you downloaded NebulaAuth from the official source:

* the application does not modify account data
* the issue is outside the application

We recommend contacting Steam Support.

***

### Steam Guard code does not work

Reason:

* the time on the PC is out of sync

Solution:

* synchronize the time with the internet
* restart the application

***

### Error when linking: BadConfirmationCode

This is a known Steam issue.

Solution:

* follow the instructions at the top of the linking window
* or see the section: [Linking → Problem solution](../getting-started/add-account/link-new.md#-solution)

***

### "Failed to synchronize time with Steam"

This error can occur when the application starts.

Reasons:

* maintenance on Steam's side
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
