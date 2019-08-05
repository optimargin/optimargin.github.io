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

[Here]({{ site.baseurl }}/docs/getting-started/files-from-fcm/) are more details about the kinds of files you need from each FCM.

### Fetching files

Set your script to routinely download new files from your FCMs. Make sure to check for new files before a scheduled full simulation run (see [initial configuration]({{ site.baseurl }}/docs/getting-started/configuration/)).

### Using shared drives

Since OptiMargin uses the LocalSystem account, if you use shared drives you might have to mount them in a way that is accessible to the LocalSystem.
<details>
<summary class="text-primary mb-3">See how</summary>
{% capture markdown %}
- download the [PSTools Suite](https://docs.microsoft.com/en-us/sysinternals/downloads/pstools) from Microsoft
- extract the folder
- search for the `Command Prompt` on the Windows menu, right click, and select `Run as administrator`
- change the directory to the folder you just downloaded and extracted
- run the command `psexec -i -s cmd.exe`. An new command window will pop up
- in the new window, run the command `net use * &lt;UNC PATH&gt; /persistent:yes`, replacing `&lt;UNC PATH&gt;` with your UNC path. If you use a username/password, use them like this: `net use * &lt;UNC PATH&gt; /user:&lt;username&gt; &lt;password&gt; /persistent:yes`
- take a note of the Drive letter assigned (for example, "Drive Z: is now connected...")
- now you can use this Drive letter in the OptiMargin App
{% endcapture %}
{{ markdown | markdownify }}
</details>