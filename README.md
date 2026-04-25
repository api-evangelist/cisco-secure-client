# Cisco Secure Client (cisco-secure-client)
Cisco Secure Client (formerly AnyConnect) is the unified endpoint agent for Cisco security and connectivity, delivering VPN, Zero Trust Network Access, endpoint posture, network visibility, and secure web access from a single installer. Programmatic interfaces are exposed indirectly through Cisco Secure Firewall, ISE, Secure Access, Umbrella, and Duo.

**URL:** [Visit APIs.json URL](https://raw.githubusercontent.com/api-evangelist/cisco-secure-client/refs/heads/main/apis.yml)

## Scope

- **Type:** Index
- **Position:** Consumer
- **Access:** 3rd-Party

## Tags:

 - Endpoint Security, Remote Access, Security, VPN, Zero Trust

## Timestamps

- **Created:** 2024-01-01
- **Modified:** 2026-04-23

## APIs

### Cisco Secure Firewall Management Center API
Configures remote-access VPN gateways, group policies, and Secure Client profiles distributed to endpoints. Authentication uses a token generated via the generatetoken endpoint and passed as the X-auth-access-token header.

**Human URL:** [https://developer.cisco.com/docs/secure-firewall-management-center-api/](https://developer.cisco.com/docs/secure-firewall-management-center-api/)

#### Tags:

 - ASA, Firewall, FTD, Management, VPN

#### Properties

- [Documentation](https://developer.cisco.com/docs/secure-firewall-management-center-api/)

### Cisco ISE ERS API
The External RESTful Services API manages the network access control plane that Secure Client integrates with for posture assessment and policy enforcement.

**Human URL:** [https://developer.cisco.com/docs/identity-services-engine/](https://developer.cisco.com/docs/identity-services-engine/)

#### Tags:

 - ERS, Identity, ISE, NAC, Posture

#### Properties

- [Documentation](https://developer.cisco.com/docs/identity-services-engine/)

### Cisco Umbrella API
Exposes the cloud-delivered DNS, secure web gateway, and roaming protection services that integrate with the Secure Client Umbrella module. Authentication uses OAuth 2.0 client credentials.

**Human URL:** [https://developer.cisco.com/docs/cloud-security/](https://developer.cisco.com/docs/cloud-security/)

#### Tags:

 - DNS, Roaming, Secure Web Gateway, Umbrella

#### Properties

- [Documentation](https://developer.cisco.com/docs/cloud-security/)

### Cisco Duo Admin API
Configures multi-factor authentication policies, users, groups, and integrations used by Secure Client deployments for ZTNA and adaptive authentication. Uses HMAC signature authentication.

**Human URL:** [https://duo.com/docs/adminapi](https://duo.com/docs/adminapi)

#### Tags:

 - Authentication, Duo, MFA, Zero Trust

#### Properties

- [Documentation](https://duo.com/docs/adminapi)

### Cisco Secure Access API
The management interface for Cisco's converged SSE platform that Secure Client connects to as a SASE endpoint agent. Endpoints cover network tunnels, ZTNA application definitions, posture profiles, and reporting.

**Human URL:** [https://developer.cisco.com/docs/cloud-security/secure-access/](https://developer.cisco.com/docs/cloud-security/secure-access/)

#### Tags:

 - SASE, Secure Access, SSE, ZTNA

#### Properties

- [Documentation](https://developer.cisco.com/docs/cloud-security/secure-access/)

## Common Properties

- [Portal](https://developer.cisco.com/)
- [Documentation](https://www.cisco.com/c/en/us/support/security/secure-client-5/series.html)
- [Getting Started](https://developer.cisco.com/docs/secure-client/getting-started/)
- [Change Log](https://www.cisco.com/c/en/us/td/docs/security/vpn_client/anyconnect/Cisco-Secure-Client-5/release/notes/release-notes-cisco-secure-client-5.html)
- [Support](https://www.cisco.com/c/en/us/support/index.html)
- [Status](https://status.cisco.com/)
- [Community](https://community.cisco.com/)
- [Terms of Service](https://www.cisco.com/c/en/us/about/legal/cloud-and-software/end-user-license-agreement.html)
- [Privacy Policy](https://www.cisco.com/c/en/us/about/legal/privacy-full.html)
- [JSON-LD Context](json-ld/cisco-secure-client-context.jsonld)
- [Spectral Ruleset](spectral/cisco-secure-client-spectral.yml)
- [Naftiko Capabilities](naftiko/cisco-secure-client-capabilities.yml)

## Maintainers

**FN:** Kin Lane

**Email:** kin@apievangelist.com
