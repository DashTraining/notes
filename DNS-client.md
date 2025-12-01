---
title: DNS Client
layout: notes
tags: [DNS]
categories: [Windows]
---

## Optimization

As name queries are resolved - one way or another - for all connections to services, they can cause performance issues on a system. Optimizing name lookups can improve almost all service communication.

* [check performance of public DNS servers](https://www.dnsperf.com/#!dns-resolvers)
* [benchmark DNS from your location](https://www.grc.com/dns/benchmark.htm)

Improvements can be made by using a fast public DNS. Configure this as your DNS server's forwarder or in your LAN router's settings. Some public options that also may offer filtering for privacy and ads removal:

* [NextDNS](https://nextdns.io/)
* [Quad9](https://quad9.net/service/service-addresses-and-features/)
* [Control D](https://controld.com/free-dns)
* [DNS4EU](https://www.joindns4.eu/for-public)
* [AdGuard DNS](https://adguard-dns.io/en/public-dns.html)

The next step is setting up the right caching on your local DNS.
