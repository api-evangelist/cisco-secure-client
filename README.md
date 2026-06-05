# Cisco Secure Client (cisco-secure-client)

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
