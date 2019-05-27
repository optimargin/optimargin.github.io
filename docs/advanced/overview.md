---
layout: docs
title: Advanced Configuration
description: "I'll have the #3, hold the onions."
group: advanced-configuration
redirect_from:
  - "/docs/advanced/"
  - "/advanced/"
  - "/docs/advanced-configuration/"
  - "/advanced-configuration/"
  - "/docs/advanced-configuration/overview/"
  - "/advanced-configuration/overview/"
toc: false
---

To access configurations, run `Open OptiMargin UI` from the Start Menu, or open a browser to `http://localhost:8080`, and click `settings`.

Click `show advanced settings...` to see all the available settings.

### Simulations settings

| setting name | description | valid values | default |
|----------------------------|----------------------------------------------------------------------------------------------------------------|-----------------|----------|
| run exchange switches | include possible recommendations: buy a fungible contract on one exchange and sell in the other | Y/N | Y |
| run fcm transfers | include possible recommendations: transfer a contract from one FCM account to another | Y/N | Y |
| run comparison vs previous | gives an analysis of the changes in margin from the previous day | Y/N | Y |