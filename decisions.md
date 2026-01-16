# Architecture Decisions

## Why not IP-based voting?
IP addresses are meaningless due to VPNs, mobile networks,
and residential proxies. They provide false confidence.

## Why token-based voting?
Voting rights must be treated like scarce digital assets.
They are minted, tracked, and burned, not inferred from identity.

## Why Cloudflare?
Cloudflare provides browser-level telemetry:
TLS fingerprints, bot scores, behavior analysis, and challenges.
This allows risk scoring without identifying users.

## Why no accounts?
Accounts are farmed, sold, and automated.
They add friction but not real security.

## Why post-hoc analysis?
Some abuse will always get through.
The system must detect and discount it after votes are cast.

## Design Principle
Security is not about blocking all attackers.
It is about making manipulation economically irrational.
