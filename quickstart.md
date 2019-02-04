---
layout:     page
title:      Quickstart
permalink: /quickstart/
---

We've released preview version `0.0.1` of **XSC Platform API**.

## XSC Platform API features

* Running at any Website without Extension setup out of the box
* Instant Transactions
* Working directly with User's local Wallet
* Open Source Software you may read to verify or modify at any time
* No Hidden comissions or Minimal fund locks
* Only Onchain payments: no proprietary gateways

## API Quickstart

Add this script to the bottom of every content page just before closing `body` tag:

{% highlight html lineanchors %}
<script src="https://api.xscp.icu/v1/widget.js"></script>
{% endhighlight %}

The result rendering

![Actual XSCP Widget rendering result](/images/widget.png)

Left Button shows **Wallet Address** bound to **Signed Content**. Wallet Address is truncated to show only 5 first and last symbols to check address if User need it. Clicking on Address calls **Payment Modal** to transfer XSCP Coins to this Address by sending **RPC API Request** directly to **Local Wallet setup**.

![XSC Platform API](/images/platform.png)

## XSCP Signature

To add on page XSCP Widget bound to your wallet address use next syntax:

{% highlight lineanchor %}
$XSCP(<your-wallet-address>)
{% endhighlight %}

You can obtain your wallet address from `Receive` GUI Wallet tab or by `getaccountaddress <account>` CLI command:

![Receive Wallet tab](/images/receive.png)

**Signature example**

<pre>
...previous content.

$XSCP(XySimjKBSSxGphzSqWcLBrxzPVMjBfwRFA)
</pre>