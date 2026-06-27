---
title: "The Big Objects Playbook: Payload Capture and Replay"
url: "https://developer.salesforce.com/blogs/2026/06/big-objects-playbook-payload-capture-and-replay"
date: "2026-06-18"
author: "Laxman Vattam"
feed_url: "https://developer.salesforce.com/blogs/feed"
---
Salesforce Big Objects store hundreds of millions of records without degrading performance and don't count against standard storage limits, making them ideal for high-volume, append-heavy, write-once-query-later workloads. The article details a two-object pattern that separates a durable payload ledger from an action queue, using Database.insertImmediate() to capture platform event payloads and Batch Apex to automate retries of failed events. The pattern applies to telecom CDRs, financial transaction history, IoT telemetry, metered billing, and marketing engagement tracking.
