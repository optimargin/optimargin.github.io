---
layout: docs
title: Initial configuration
description: This should take a minute.
group: getting-started
toc: false
redirect_from:
  - "/docs/getting-started/initial-configuration/"
  - "/getting-started/initial-configuration/"
---

To access configurations, run `Open OptiMargin UI` from the Start Menu, or open a browser to `http://localhost:8080`, and click `settings`.

Click `show advanced settings...` to see all the available settings.

### General settings

| setting name | description | valid values | default |
|----------------------------|----------------------------------------------------------------------------------------------------------------|-----------------|----------|
| run automatically | run a full simulation (and send emails) daily at the specified time | Y/N | Y |
| start time | time at which to start the daily simulation | HH:MM AM/PM | 05:00 AM |
| interest rate | annualized interest rate used to calculate cost of borrowing margin requirement | decimal | 0.04 |

### Email settings

| setting name | description | valid values | default |
|----------------------------|----------------------------------------------------------------------------------------------------------------|-----------------|----------|
| send automatic email | send email automatically after the daily run | Y/N | Y |
| to, from, cc | sender/recipient fields on the email | valid emails |  |
| host, port | used to send the email. Mailchimp (Mandrill) integration coming soon |  |  |

### FCM settings

For each FCM:

| setting name | description | valid values | default |
|----------------------------|----------------------------------------------------------------------------------------------------------------|-----------------|----------|
| directory | path to directory with position and IM files | string | `C:\data` |
| position file name | naming convention in regex format, for example `\d{8}_STANDARD POSITION FILE\.xlsx` | string |  |
| IM file name | naming convention in regex format, for example `\d{8}_BRKDWN_FUT_INITLMGN\.csv` | string |  |