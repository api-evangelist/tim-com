# TIM (tim-com)

TIM S.p.A. (formerly Telecom Italia) is the incumbent Italian telecommunications operator and parent of TIM Brasil, the second-largest mobile operator in Brazil. The group exposes its mobile network as a programmable platform through the `developer.tim.it` portal in Italy and TIM Open Gateway in Brazil, both implementing CAMARA-standard network APIs (SIM Swap, Number Verification, Know Your Customer, IP-to-MSISDN, IP-to-Number, Device Location) jointly defined by the Linux Foundation, TM Forum, and GSMA.

**URL:** [Visit APIs.json](https://raw.githubusercontent.com/api-evangelist/tim-com/refs/heads/main/apis.yml)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=company-api-evangelist&utm_content=repo)

## Tags

- Telecommunications, Telco, Mobile Network Operator, Network APIs, CAMARA, Open Gateway, GSMA, SIM Swap, Number Verification, Know Your Customer, Identity, Anti-Fraud, Italy, Brazil, 5G

## Timestamps

- **Created:** 2026-05-25
- **Modified:** 2026-05-25

## APIs

### TIM SIM Swap
CAMARA-aligned API returning the timestamp of the last SIM swap (or whether one occurred within a caller-supplied window) for a TIM mobile number. Used by banks and fintechs as a signal against account-takeover fraud.

**Human URL:** [https://developer.tim.it/security/TIM%20SIM%20Swap/dev](https://developer.tim.it/security/TIM%20SIM%20Swap/dev)

- [Documentation (Italy)](https://developer.tim.it/security/TIM%20SIM%20Swap/dev)
- [Documentation (Brazil)](https://www.tim.com.br/open-gateway/sim-swap)
- [CAMARA SimSwap reference](https://github.com/camaraproject/SimSwap)

### TIM Number Verification
CAMARA Number Verification API that silently confirms the MSISDN bound to the active mobile data session against the number asserted by the application. Replaces SMS-OTP with passive carrier-grade verification.

**Human URL:** [https://developer.tim.it/security/TIM%20Number%20Verification/dev](https://developer.tim.it/security/TIM%20Number%20Verification/dev)

- [Documentation (Italy)](https://developer.tim.it/security/TIM%20Number%20Verification/dev)
- [Documentation (Brazil)](https://www.tim.com.br/open-gateway/number-verify)
- [CAMARA NumberVerification reference](https://github.com/camaraproject/NumberVerification)

### TIM Know Your Customer - Match
KYC Match API that compares customer-supplied attributes (name, tax ID, date of birth, address) against TIM's subscriber records and returns per-attribute match scores. Used during onboarding to validate identity claims and reduce manual KYC review.

**Human URL:** [https://developer.tim.it/security/TIM%20Know%20Your%20Customer%20-%20Match/dev](https://developer.tim.it/security/TIM%20Know%20Your%20Customer%20-%20Match/dev)

- [Documentation (Italy)](https://developer.tim.it/security/TIM%20Know%20Your%20Customer%20-%20Match/dev)
- [Documentation (Brazil)](https://www.tim.com.br/open-gateway/know-your-customer)
- [CAMARA KnowYourCustomer reference](https://github.com/camaraproject/KnowYourCustomer)

### TIM IP to MSISDN
Given an IP address observed by a relying party, returns the TIM mobile number (MSISDN) currently associated with that radio session. Used by banking and payment apps to bind in-app actions to a known mobile number without an OTP round-trip.

**Human URL:** [https://developer.tim.it/security/TIM%20IP%20to%20MSISDN/dev](https://developer.tim.it/security/TIM%20IP%20to%20MSISDN/dev)

- [Documentation](https://developer.tim.it/security/TIM%20IP%20to%20MSISDN/dev)

### TIM IP to Number
Given an IP address, returns the TIM fixed-line or mobile number associated with the session. Extends IP-to-MSISDN to cover both mobile and broadband subscribers for fraud and access-control use cases.

**Human URL:** [https://developer.tim.it/security/TIM%20IP%20to%20Number/dev](https://developer.tim.it/security/TIM%20IP%20to%20Number/dev)

- [Documentation](https://developer.tim.it/security/TIM%20IP%20to%20Number/dev)

### TIM Device Location
CAMARA Device Location verification API offered by TIM Brasil Open Gateway. Confirms whether a mobile device is physically within a supplied geographic area at request time, supporting geofenced authentication and fraud checks.

**Human URL:** [https://www.tim.com.br/open-gateway/device-location](https://www.tim.com.br/open-gateway/device-location)

- [Documentation](https://www.tim.com.br/open-gateway/device-location)
- [CAMARA DeviceLocation reference](https://github.com/camaraproject/DeviceLocation)

## Common

- [Website — TIM Group](https://www.gruppotim.it/en.html)
- [Website — TIM Italy](https://www.tim.it)
- [Website — TIM Brasil](https://www.tim.com.br)
- [Portal — TIM Developer Portal (Italy)](https://developer.tim.it)
- [Portal — TIM Open Gateway (Brazil)](https://www.tim.com.br/open-gateway)
- [TIM API Catalog](https://developer.tim.it/apis-developer)
- [Standard — CAMARA Project (Linux Foundation)](https://camaraproject.org/)
- [About — TIM Group](https://www.gruppotim.it/en/group.html)
- [Press Release — TIM Brasil Open Gateway launch](https://www.tim.com.br/sobre-a-tim/sala-de-imprensa/press-releases/institucional/tim-lanca-novas-apis)
- [Subsidiary — Sparkle](https://www.tisparkle.com/)
- [Subsidiary — Noovle](https://www.noovle.com/)
- [Subsidiary — Telsy](https://www.telsy.com/)
- [Subsidiary — Olivetti](https://www.olivetti.com/)
- [Investor Relations](https://www.gruppotim.it/en/investors.html)
- [Careers](https://www.gruppotim.it/en/careers.html)
- [LinkedIn](https://www.linkedin.com/company/tim-official-page/)
- [Twitter](https://twitter.com/TIMnewsroom)
- [YouTube](https://www.youtube.com/user/TIM)

## Maintainers

- **Kin Lane** — kin@apievangelist.com
