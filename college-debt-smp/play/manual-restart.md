---
description: When the server is not awake for some reason
noIndex: true
icon: arrows-rotate
---

# Manual restart

The server by itself should always be available for the majority of the time. If you need to manually reboot it for whatever reason, keep reading.

{% hint style="info" %}
Before proceeding further, ensure that the server is not intentionally down for a planned maintenance.
{% endhint %}

{% stepper %}
{% step %}
Log into the [container management interface](https://cmi.cherri.qzz.io/) with your Cloud Debt account
{% endstep %}

{% step %}
Navigate to <i class="fa-docker">:docker:</i> **Ampere** → <i class="fa-cube">:cube:</i> **Containers** → **cdsmp**
{% endstep %}

{% step %}
Click on <i class="fa-arrows-rotate">:arrows-rotate:</i> **Restart**
{% endstep %}

{% step %}
Wait until the container turns healthy. Optionally, look at the container log to ensure graceful start.
{% endstep %}
{% endstepper %}
