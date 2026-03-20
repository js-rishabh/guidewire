🌩️ StormSafe
Parametric Weather Insurance for Gig Workers

DEVTrails 2026 | Phase 1 Submission

📑 Table of Contents

1.Problem Statement Breakdown
2.Adversarial Defense & Anti-Spoofing Strategy
    2.1 The Differentiation (Architecture, Flows, Tables)
    2.2 The Data
    2.3 The UX Balance
3.Conclusion


1. 🚨 Problem Statement Breakdown
1.1 The Gig Economy Reality
India’s gig economy consists of 15M+ delivery workers operating under high uncertainty. During severe weather events such as:

Cyclones
Flash floods
Thunderstorms

workers face a binary choice:

| Option           | Outcome            |
| ---------------- | ------------------ |
| Continue working | Risk life & safety |
| Stop working     | Lose daily income  |

1.2 Why Traditional Insurance Fails

Traditional insurance models are not viable because:

    Require manual claims
    Need proof collection (impossible during storms)
    Slow settlement cycles (days/weeks)
    High friction for low-income workers

1.3 Parametric Insurance — The Ideal Solution

Parametric insurance solves this via:
    IF weather trigger == TRUE
    THEN payout automatically

Example:

    IMD Red Alert in a region
    Rainfall threshold exceeded

    ✔ No paperwork
    ✔ No claim filing
    ✔ Payout in ~90 seconds

1.4 The Critical Vulnerability

⚠️ The 500-Worker Syndicate Attack
A coordinated fraud ring exploited the system by:

    Using GPS spoofing apps
    Simulating presence in storm zones
    Coordinating via Telegram
    Triggering mass false claims

Result:
    Entire liquidity pool drained
    System collapse

1.5 Root Cause

The failure stems from:
❌ Single Point of Failure: GPS

| Assumption            | Reality               |
| --------------------- | --------------------- |
| GPS = Truth           | GPS is spoofable      |
| One device = one user | Device farms exist    |
| Location = presence   | Location can be faked |

1.7 Core Problem Statement

How do we verify that a worker is physically present in a dangerous weather environment — in real-time — in a way that cannot be spoofed at scale?
