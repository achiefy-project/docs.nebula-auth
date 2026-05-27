# Using proxies in accounts

### Assigning a proxy

![Assigning a proxy](../../../.gitbook/assets/mw-set-proxy.png)

To assign a proxy to an account:

1. Select the required account
2. In the **"Proxy"** field at the top, select the required proxy from the dropdown list

When switching between accounts, you will see the assigned proxy.

The proxy is stored inside the **maFile**, so when transferring the file between different NebulaAuth instances, it will also be preserved.

***

### Where the proxy is used

The proxy is applied when the account works with:

* authorization and session
* confirmations
* auto-confirmations

***

### Removing a proxy from an account

To unbind a proxy from an account:

**Method 1:**

1. Click the **"Proxy"** field
2. Press the **DEL** key

**Method 2:**

1. Right-click the account
2. Select **"Unbind proxy"**

After that, the account will use the default proxy, if it is set, or work directly.

***

### Default proxy

If the account does not have its own proxy assigned, the default proxy is used.

```
account proxy → default proxy → direct
```

This lets you define common network behavior and avoid working without a proxy.

***

### Use during linking and transfer

When **linking an account** or **transferring Steam Guard**, you can select a proxy from the list.

The selected proxy:

* is used while the operation is being performed
* is automatically saved in the created maFile

***

### Indicators in the interface

The interface displays proxy states:

* red, if the proxy is used from the account but is missing in the manager
* yellow, if the account works through the default proxy