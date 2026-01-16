# Threat Model – Anti-Abuse Voting System

## Objective
Prevent large-scale manipulation of voting outcomes in an open,
anonymous, web-based system.

## Primary Adversaries

### 1. Script Bots
Simple HTTP or JS-based automation attempting to mass mint tokens
and submit votes.

### 2. Headless Browsers
Playwright / Puppeteer style browsers that can pass basic CAPTCHA
and mimic human behavior.

### 3. Proxy Networks
Residential and mobile IP networks used to bypass IP-based limits.

### 4. Human Click Farms
Low-paid humans performing real browser interactions at scale.

---

## Attacker Goals

- Mass token acquisition
- Outcome manipulation
- Statistical distortion
- Bypassing rate limits and detection

---

## Defender Constraints

- No KYC
- No phone or email verification
- Open public access
- Web browser only

---

## Key Insight

Attackers will not try to guess tokens.
They will try to harvest them from the minting pipeline.

Therefore:
**The minting process is the primary battlefield.**
