---
description: For administrator working on the server settings
icon: toolbox
---

# Admin toolbox

{% hint style="warning" %}
If you don't know what you're looking at, this page does not apply to you
{% endhint %}

This page list additional tools and materials available for administration purposes.

## Server Cluster

<details>

<summary>Cloudflare Dashboard</summary>

DNS routing, TLS settings, and SSO configurations for some site are on the Cloudflare dashboard of the server. Request CherryQuartzio for permission to access.

Link is available on the Server Dashboard

</details>

<details>

<summary>Server nodes</summary>

The following machine node are currently operable on the server

<table><thead><tr><th width="120.2666015625">Hostname</th><th width="119.39996337890625">Provider</th><th>Specification</th></tr></thead><tbody><tr><td>oci-arm-cq</td><td>Oracle Cloud</td><td><ul><li>Ampere Altra 80C (4 cores) @ 3.0 GHz (aarch64)</li><li>24GB memory</li><li>100GB internal storage</li><li>Ubuntu Server</li></ul></td></tr></tbody></table>

Admin users can directly log into a node's Linux terminal using SSH. To do so, the remote machine must be connected to the Server VPN.

The server is designed to be expandable. In other words, additional Linux machine with Docker can be added as a worker node to be managed centrally by the control node. The option to use Kubernetes is also possible. Tailscale can be use to communicate with nodes from a different location.

</details>

<details>

<summary>Visual Studio Code</summary>

An instance of VS Code server is running on the server node to allow ease of editing config file for some services directly from your local VS Code client. You need the _Remote - SSH_ extension installed.

All editable config files are in its respective service directory, which all are located in the server user account home directory.

Additionally, you can also access bash as well. The Server Cluster was configured with heavy reliance on Docker. In most cases, you should not need to change any system settings of the node outside of configuring the Docker Runtime or the Tailscale connection of the node.

</details>

## Cloud Debt 365

<details>

<summary>Microsoft Admin interfaces</summary>

Microsoft splits the management of certain aspect of the tenant into multiple interfaces. Below are the services that the College Debt SMP and the Server Cluster uses:

* [Entra](https://entra.microsoft.com/): SSO configuration

- [Sharepoint](https://sheldonbois-admin.sharepoint.com/): Group-wide data storage
- [Exchange](https://admin.exchange.microsoft.com/?landingpage=mailboxes\&form=mac_sidebar): Email management

</details>
