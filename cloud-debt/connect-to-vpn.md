---
description: Connecting to the server's Tailscale network
icon: circle-wifi-circle-wifi
---

# Connect to VPN

To securely access the server and join using the Tailscale network address, you need to connect to the Server Cluster through a VPN.



1. Download the [Tailscale client](https://tailscale.com/download) for your device
2. Connect the client to the Server Cluster address depending on your platform

<details>

<summary>Android</summary>

* Open the app and select the settings menu in the upper-right corner
* Tap on `Accounts`
* In the kebab menu icon (three dots) in the upper-right corner select `Use an alternate server`
* Enter your server URL (e.g `https://headscale.example.com`) and follow the instructions

</details>

<details>

<summary>iOS/iPadOS</summary>

* Open the Tailscale app
* Click the account icon in the top-right corner and select `Log in…`.
* Tap the top-right options menu button and select `Use custom coordination server`.
* Enter the following url: `https://hs.sheldonbois.dpdns.org`
* Continue

</details>

<details>

<summary>macOS</summary>

* Option + Click the Tailscale icon in the menu and hover over the Debug menu
* Under `Custom Login Server`, select `Add Account...`
* Enter the url `https://hs.sheldonbois.dpdns.org` and press `Add Account`
* Continue in the browser

</details>

<details>

<summary>Windows</summary>

Open a Windows Terminal or Powershell and type in the following command

```
tailscale login --login-server https://hs.sheldonbois.dpdns.org
```

Follow the instructions in the opened browser window

</details>

3. Authenticate using your Cloud Debt 365 account
