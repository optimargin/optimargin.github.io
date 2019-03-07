---
layout: docs
title: Installing OptiMargin
description: 1, 2, 3... done!
group: getting-started
toc: false
redirect_from:
  - "/docs/getting-started/installing-optimargin/"
  - "/getting-started/installing-optimargin/"
---

To install OptiMargin, you need to run the installer with administrator privileges

<details>
<summary class="text-primary mb-3">Running as administrator</summary>
{% capture markdown %}
- right click the OptiMargin installer
- click `Run as administrator`
- you might have to enter your password. Click `Yes`
{% endcapture %}
{{ markdown | markdownify }}
</details>

By default, the OptiMargin App sends error logs (with absolutely **no** user data) to our IT team in order to more quickly identify and resolve potential problems. If you would rather disable this feature and have no outgoing logs, click `Advanced` during the installation process and uncheck `Automatically send diagnostic error logs`.

During the installation process, please enter the `client id` and `password` provided by the OptiMargin team.

After installation, OptiMargin will run automatically.

To stop OptiMargin, run `Stop OptiMargin Services` from the Start Menu.

To start OptiMargin again, run `Start OptiMargin Services` from the Start Menu.