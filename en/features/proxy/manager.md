# Proxy manager

Open the proxy manager from Menu **→ Proxy manager**.

![Proxy manager](../../../.gitbook/assets/proxy-manager.png)

***

### ⚙️ Capabilities

In the proxy manager you can:

* add proxies
* delete proxies
* assign a default proxy
* copy a full proxy entry or only its address

***

### ✏️ Entering a proxy

Supported formats:

```id="proxy-formats"
IP:PORT
IP:PORT:USER:PASS
USER:PASS@IP:PORT
protocol://IP:PORT
protocol://USER:PASS@IP:PORT
```

The default protocol is **HTTP**.

{% hint style="info" %}
For **SOCKS4 / SOCKS5** proxies, the protocol must be explicitly specified, for example: `socks5://IP:PORT`.
{% endhint %}

***

#### 🆔 Using ID

When adding a proxy, you can specify an ID in curly braces:

```id="kq7s2p"
IP:PORT:USER:PASS{0}
```

The ID makes proxy management easier by letting you quickly identify a proxy by number.

All lines must contain a unique ID. If the specified ID already exists, the corresponding proxy will be **overwritten**.

***

#### 🌐 Default proxy

You can assign a default proxy.

It is used as a fallback: if an account does not have its own proxy assigned, requests go through the default proxy. If neither an account proxy nor a default proxy is set, requests are sent directly.

```
account proxy → default proxy → direct
```

The default proxy is useful when you want to control network requests and avoid working without a proxy.

If you delete the proxy assigned as the default, the application stops using it and works directly for accounts that do not have their own proxies.

{% hint style="info" %}
If you need to completely prevent direct connections, you can specify a deliberately non-working proxy, for example `0.0.0.0:5555`.

In this case, accounts with an assigned proxy will work as usual, while the others will not be able to send requests directly.
{% endhint %}

***

### ❓ Frequently asked questions

<details>

<summary><strong>What will happen if I delete a proxy from the manager?</strong></summary>

The proxy is not deleted from the maFile.

The account keeps the attachment, but when you select this account, a red "Using proxy from maFile" icon is displayed. To fully unattach the proxy, remove the attachment from the account itself.

</details>

<details>

<summary><strong>Where are proxies stored?</strong></summary>

Proxies from the manager are stored in the `proxies.json` file in the root of the application folder. The proxy attachment to the account is stored in that account's maFile.

</details>

<details>

<summary><strong>Can I import proxies from a file?</strong></summary>

There is no direct import, but you can easily add proxies from any text file:

1. Open the file with proxies
2. Copy the list
3. Paste it into the proxy manager

</details>

<details>

<summary><strong>Can I export proxies?</strong></summary>

There is no direct export, but you can easily copy proxies from the manager:

1. Right-click the required proxy
2. Select "Copy" or "Copy address"

</details>

<details>

<summary><strong>Can I edit proxies?</strong></summary>

There is no direct editing, but you can overwrite a proxy by adding a new entry with the same ID.

</details>

<details>

<summary><strong>Is there a limit on the number of proxies?</strong></summary>

No.

You can add any number of proxies.

</details>

***

In the next section, we will look at how to use added proxies when working with accounts.

{% content-ref url="usage.md" %}
[usage.md](usage.md)
{% endcontent-ref %}
