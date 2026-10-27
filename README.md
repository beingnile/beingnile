## Hey, I'm Nile

I'm a backend engineer. By day that's mostly payments, routers and RADIUS servers. By night I try to break the stuff I built by day.

I founded [NetBill](https://netbill.app) in February 2025, billing and router provisioning for small ISPs in Kenya. 115 businesses have signed up since. The hardest problem has been routers stuck behind carrier-grade NAT, so now the router makes every connection itself: it registers, pulls its config and sends a heartbeat every two minutes. RouterOS fought me the whole way. My one-line onboarding command threw "No such item" on factory-fresh routers, and I ended up rewriting every generated script without a single `{ }` block.

I also freelance, writing Go and Python for [StrataxIQ](https://strataxiq.com). Until October 2026 I built M-Pesa ticketing for Zuka, and I still do occasional maintenance there. On the side I'm building [Sheaf](https://sheaf.co.ke), social commerce for SMEs on a monthly subscription. It's in development and testing now. I'm also building [Coffee Beans](https://coffeebeans.tweeps.co.ke), a hospitality management system, with an accountant.

A few things I'm proud of:

- An Apple MDM protocol server in Go, with a tamper-evident audit log that verifies its own hash chain every hour
- M-Pesa integrations with idempotent callbacks, Redis locks against double booking, and HMAC-signed tickets
- A guest WiFi captive portal on FreeRADIUS that works across MikroTik, UniFi and Meraki

The bug I learned the most from was in my own M-Pesa code. The webhook trusted the `CF-Connecting-IP` header, but the origin server was reachable directly, so anyone could fake a payment. While fixing it I also found a payout that could be sent twice. Now I write up the security side on [Medium](https://medium.com/@beingnile): 97+ articles so far on HTB boxes, privesc and SQLi, plus whatever I'm working through on PortSwigger and pwn.college.

Most of my client work is private. If you want to see how something works, just ask. NetBill is stable and needs a few hours a week, so I'm looking for an application security role as my main focus, preferably remote.

Away from the keyboard: guitar, music and chess.

[Portfolio](https://nile-okomo.vercel.app) · [LinkedIn](https://linkedin.com/in/nile-okomo) · okomonile3@gmail.com
