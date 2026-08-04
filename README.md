# TIM (tim-com)

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

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
