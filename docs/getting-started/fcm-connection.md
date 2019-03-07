---
layout: docs
title: Connecting to your FCMs
description: Your positions are automatically updated.
group: getting-started
redirect_from:
  - "/docs/getting-started/connecting-to-your-fcms/"
  - "/getting-started/connecting-to-your-fcms/"
---

{%- comment -%}
Although you can manually add files to [run simulations](/link-to-simulations-explanation), we strongly recommend you set up FTP connections with your FCMs to automate the process.
{%- endcomment -%}

### Setup

This whole process consists of **requesting an FTP connection** with your FCM(s) and writing a quick and easy **script** to periodically update your position/IM files. *We are happy to take care of this for you if needed*.

### Connection

Setting up an FTP connection to your FCM is straight-forward and should take approximately one week (depending on your FCM). You should request two kinds of files in either *csv* or *xls(x)* format (PDF is also supported, but not recommended):
- Position files: lists your current cumulative positions
- IM files: lists how much money you are currently being charged in maintenance margin.

### Fetching files

Set your script to routinely download new files from your FCMs. Make sure to check for new files before a scheduled full simulation run (see [initial configuration]({{ site.baseurl }}/docs/getting-started/configuration/)).

### File formats

The file formats for the following FCMs are currently supported for automatic parsing:
<div class="half-table">
{% capture markdown %}

| FCM              |
|:----------------:|
| ABN              |
| BNP              |
| Citi             |
| Societe Generale |

{% endcapture %}
{{ markdown | markdownify }}
</div>

If your FCM is not shown, please send example files to [{{ site.help_email }}](mailto: {{ site.help_email }}) and we will quickly add support for it. The position/IM sample files can either old files or position/IM files with redacted information.