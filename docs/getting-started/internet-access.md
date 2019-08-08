---
layout: docs
title: Internet access.
description: Need to configure your firewall?
group: getting-started
---

This is how OptiMargin App uses the internet.

### Receiving Data
- ftp://ftp.cmegroup.com - risk array data
- https://theice.com - risk array data
- https://quandl.com - get market data, such as Treasury rates
- https://api.optimargin.com - software updates and market data for switches

### Sending Data
- *OPTIONAL* https://api.optimargin.com - send error logs
- *OPTIONAL* https://mandrillapp.com/api - send the daily emails (you can use your internal mail server instead)