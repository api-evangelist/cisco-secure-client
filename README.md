# Cisco Secure Client (cisco-secure-client)

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

Cisco Secure Client (formerly AnyConnect) is the unified endpoint agent for Cisco security and connectivity, delivering VPN, Zero Trust Network Access, endpoint posture, network visibility, and secure web access from a single installer. Programmatic interfaces are exposed indirectly through Cisco Secure Firewall (ASA, FTD), Cisco Identity Services Engine (ISE), Cisco Secure Access, Umbrella, and Duo. There is no single public REST surface for the client itself; integration is achieved through profile XML packages, MDM-deployed configuration, and the management plane APIs exposed by these adjacent Cisco services.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/cisco-secure-client/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/cisco-secure-client/refs/heads/main/apis.yml)

## Scope

- **Type:** Index
- **Position:** Consumer
- **Access:** 3rd-Party

## Tags

- Endpoint Security
- Remote Access
- Security
- VPN
- Zero Trust

## Timestamps

- **Created:** 2024-01-01
- **Modified:** 2026-04-23

## APIs

### Cisco Secure Firewall Management Center API

The Cisco Secure Firewall Management Center API configures remote-access VPN gateways, group policies, and Secure Client profiles distributed to endpoints. Authentication uses a token generated via the generatetoken endpoint and passed as the X-auth-access-token header on subsequent calls.

- **Human URL:** [https://developer.cisco.com/docs/secure-firewall-management-center-api/](https://developer.cisco.com/docs/secure-firewall-management-center-api/)

#### Tags

- ASA
- Firewall
- FTD
- Management
- VPN

#### Properties

- [Documentation](https://developer.cisco.com/docs/secure-firewall-management-center-api/)
- [Postman Collection](collections/cisco-secure-client.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/cisco-secure-client.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Cisco ISE ERS API

The Cisco Identity Services Engine External RESTful Services (ERS) API manages the network access control plane that Secure Client integrates with for posture assessment and policy enforcement. Endpoints cover endpoint identity groups, posture conditions, and authorization policies.

- **Human URL:** [https://developer.cisco.com/docs/identity-services-engine/](https://developer.cisco.com/docs/identity-services-engine/)

#### Tags

- ERS
- Identity
- ISE
- NAC
- Posture

#### Properties

- [Documentation](https://developer.cisco.com/docs/identity-services-engine/)
- [Postman Collection](collections/cisco-secure-client.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/cisco-secure-client.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Cisco Umbrella API

The Cisco Umbrella API exposes the cloud-delivered DNS, secure web gateway, and roaming protection services that integrate with the Secure Client Umbrella module. Authentication uses OAuth 2.0 client credentials and endpoints cover deployments, policies, reports, and destination lists.

- **Human URL:** [https://developer.cisco.com/docs/cloud-security/](https://developer.cisco.com/docs/cloud-security/)
- **Base URL:** `https://api.umbrella.com`

#### Tags

- DNS
- Roaming
- Secure Web Gateway
- Umbrella

#### Properties

- [Documentation](https://developer.cisco.com/docs/cloud-security/)
- [Postman Collection](collections/cisco-secure-client.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/cisco-secure-client.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Cisco Duo Admin API

The Duo Admin API configures multi-factor authentication policies, users, groups, and integrations used by Secure Client deployments for ZTNA and adaptive authentication. Authentication uses an HMAC signature scheme over the request and integration keys.

- **Human URL:** [https://duo.com/docs/adminapi](https://duo.com/docs/adminapi)

#### Tags

- Authentication
- Duo
- MFA
- Zero Trust

#### Properties

- [Documentation](https://duo.com/docs/adminapi)
- [Postman Collection](collections/cisco-secure-client.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/cisco-secure-client.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Cisco Secure Access API

The Cisco Secure Access API is the management interface for Cisco's converged SSE platform that Secure Client connects to as a SASE endpoint agent. Endpoints cover network tunnels, ZTNA application definitions, posture profiles, and reporting.

- **Human URL:** [https://developer.cisco.com/docs/cloud-security/secure-access/](https://developer.cisco.com/docs/cloud-security/secure-access/)

#### Tags

- SASE
- Secure Access
- SSE
- ZTNA

#### Properties

- [Documentation](https://developer.cisco.com/docs/cloud-security/secure-access/)
- [Postman Collection](collections/cisco-secure-client.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/cisco-secure-client.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [Portal](https://developer.cisco.com/)
- [Documentation](https://www.cisco.com/c/en/us/support/security/secure-client-5/series.html)
- [Getting Started](https://developer.cisco.com/docs/secure-client/getting-started/)
- [Changelog](https://www.cisco.com/c/en/us/td/docs/security/vpn_client/anyconnect/Cisco-Secure-Client-5/release/notes/release-notes-cisco-secure-client-5.html)
- [Support](https://www.cisco.com/c/en/us/support/index.html)
- [Status Page](https://status.cisco.com/)
- [Community](https://community.cisco.com/)
- [Terms of Service](https://www.cisco.com/c/en/us/about/legal/cloud-and-software/end-user-license-agreement.html)
- [Privacy Policy](https://www.cisco.com/c/en/us/about/legal/privacy-full.html)
- [JSON-LD](json-ld/cisco-secure-client-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)
- [Spectral Rules](rules/cisco-secure-client-rules.yml) — [Spectral](https://docs.stoplight.io/docs/spectral)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
