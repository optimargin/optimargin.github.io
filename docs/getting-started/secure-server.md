---
layout: docs
title: Setting up a secure server
description: You are the only custodian for your data.
group: getting-started
toc: false
redirect_from:
  - "/docs/getting-started/setting-up-a-secure-server/"
  - "/getting-started/setting-up-a-secure-server/"
---

Let's set up a secure server that only **you** have access to.

### Server Specs
We recommend using either Windows Server 2016/2019 (desktop experience) or Windows 10.

A more powerful server will deliver your results much faster.

<div class="half-table">
{% capture markdown %}

| minimum | recommended |
|:-----------------:|:-------------------:|
| 4 cores, 8 GB RAM | 16 cores, 32 GB RAM |

{% endcapture %}
{{ markdown | markdownify }}
</div>

## Where to host the server

### In-house

Your IT team creates and manages either a physical or a virtual server.

This is potentially the more secure option, since all the data never leaves your servers.

### Cloud-hosted

We set up the server for you on a secure [Google Cloud](https://cloud.google.com/) instance. We seal off access and hand over the keys to you. We will have **no access** to your server, unless you give us temporary access for maintenance.

This is potentially the more reliable option, since Google is responsible for the server being always available and fully functional.