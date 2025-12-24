---
description: The goodies in our homelab
hidden: true
noIndex: true
icon: grid-dividers
cover: >-
  https://images.unsplash.com/photo-1605745341075-1b7460b99df8?crop=entropy&cs=srgb&fm=jpg&ixid=M3wxOTcwMjR8MHwxfHNlYXJjaHw4fHxkb2NrZXJ8ZW58MHx8fHwxNzU1NTMzNjkxfDA&ixlib=rb-4.1.0&q=85
coverY: 155.01205519361952
layout:
  width: default
  cover:
    visible: true
    size: full
  title:
    visible: true
  description:
    visible: true
  tableOfContents:
    visible: true
  outline:
    visible: true
  pagination:
    visible: true
  metadata:
    visible: true
---

# Web Services

The Server Cluster runs the College Debt SMP as well as additional multiplayer servers and other self-hosted software. Available on the dashboard, these services are for members to use for their own benefit and are not meant for a production environment.

This list will update accordingly to what is currently deployed on the server.

<table><thead><tr><th width="125.43328857421875">Name</th><th>Purpose</th></tr></thead><tbody><tr><td><a href="https://docs.craftycontrol.com/">Crafty Controller</a></td><td>Quickly create and manage Minecraft servers. They are intended for running custom maps or short-term survival world.</td></tr><tr><td><a href="https://docs.n8n.io/">n8n</a></td><td>Provide the ability to create workflow automation between different SaaS apps including self-hosted one. This can be very useful in aiding your productivity process.</td></tr><tr><td><a href="https://freshrss.github.io/FreshRSS/en/">FreshRSS</a></td><td>RSS news feed aggregator. It gives you a nice alternative to manage your news feed without relying on third party services, which can have questionable quality and ease of use lately.</td></tr></tbody></table>

## Administrative tools

These services are used to manage and configure core functionality of the Server Cluster. Non-administrative members should not change anything in them, as they offer no productivity purposes.

The documentation for each of these apps can be found from their respective website and/or code repository on GitHub.

<table><thead><tr><th width="122.800048828125">Name</th><th>Purpose</th></tr></thead><tbody><tr><td><a href="https://docs.goauthentik.io/docs/"><del>Authentik</del></a></td><td><del>SSO and access control. We utilized this to manage who can access to which service on the server and prevent strangers from getting in.</del><br><br>As of now, SSO are managed by Cloudflare Access and Entra ID directly. This service is not running, but might be useful in the future.</td></tr><tr><td><a href="https://developers.cloudflare.com/cloudflare-one/">Cloudflare</a></td><td>DNS routing and Zero Trust management. We primarily use Tunnels to expose server apps onto the public address.<br><br>This service is provided externally from the Server Cluster.</td></tr><tr><td><a href="https://nginxproxymanager.com/">Nginx Proxy Manager</a></td><td>Local reverse proxy directly linked to the https port on the server host. We used this in cases where a service doesn't behave properly through the Cloudflare Zero Trust Tunnel.</td></tr><tr><td><a href="https://docs.portainer.io/sts/user/docker">Portainer</a></td><td>Docker container management for everything running on the server. In addition, the management interface also support managing Kubernetes cluster.</td></tr><tr><td><a href="https://tailscale.com/kb/1348/guides">Headplane</a></td><td>We used a self-hosted instance of Tailscale known as Headscale for VPN connections. The network, also known as a Tailnet, can be manage using the Headplane app. Device management, key generation, and access control is the same as the official Tailscale admin panel.</td></tr></tbody></table>

Additionally, we also rely on Microsoft Entra ID from Cloud Debt 365 for SSO authentication.

## Hosting request

If there's any software that you would like to self-host but don't have the resource to, you may request to have it be hosted on the Server Cluster. Due to available computing power and security implication, it must meet the following criteria:

* Be available as a Docker image that supports the arm64/aarch64 architecture
* Have a good amount of reputation from the community and other users
* Meet [Oracle Cloud Services Agreement](https://www.oracle.com/contracts/docs/cloud_csa_v012418_sg_eng_4419911.pdf)

Resource demanding services may require a cluster expansion to maintain performance target, in which you must partake in contributing a server node for the Server Cluster unless you already have done so. As this is a community effort, we want to ensure optimal access for all.
