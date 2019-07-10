---
layout: docs
title: Files from your FCMs
description: What files do I need?
group: getting-started
redirect_from:
  - "/docs/getting-started/files-from-your-fcms/"
  - "/getting-started/files-from-your-fcms/"
---

There are 2 files that you need to fetch from your FCM every day.

#### 1. Position File

This is a snapshot of the positions in your portfolio. It should include for each position:

<div class="half-table">
{% capture markdown %}

| Columns                         |
|:-------------------------------:|
| exchange (CME, ICE, NDQ, etc)   |
| product code                    |
| contract month (or day)         |
| quantity                        |
| type (future, call, put, etc)   |
| strike (if applicable)          |

{% endcapture %}
{{ markdown | markdownify }}
</div>

#### 2. IM File

Any file that includes the **total amount of margin** being currently charged by your FCM.

## Currently Supported FCMs

The file formats for the following FCMs are currently supported for automatic parsing:
<div class="half-table">
{% capture markdown %}

| FCM              |
|:----------------:|
| ABN              |
| BNP              |
| Citi             |
| ED&F             |
| Societe Generale |

{% endcapture %}
{{ markdown | markdownify }}
</div>

**If your FCM is not shown**, please send example files to [{{ site.help_email }}](mailto: {{ site.help_email }}) and we will quickly add support for it. The position/IM sample files can be either old files or position/IM files with redacted information.