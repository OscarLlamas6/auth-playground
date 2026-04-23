# Auth Playground

> Laboratorio práctico de ~89 métodos y protocolos de autenticación.
> Cada subcarpeta contiene una implementación mínima (servidor + cliente), notas de aprendizaje
> y un análisis de vulnerabilidades comunes.

---

## Leyenda de estados

| Emoji | Estado | Significado |
|-------|--------|-------------|
| 🟢 | Vigente | Estándar activo, recomendado para uso en producción |
| 🟡 | Legacy pero en uso | Todavía presente en sistemas reales; evitar en diseños nuevos |
| 🔵 | Emergente / Nuevo 2025-2026 | En adopción activa o estandarización reciente |

---

## Índice de categorías

- [`01-http-auth-basics/`](./01-http-auth-basics/) — **HTTP Auth Basics** (6 métodos): Fundamentos de autenticación HTTP: Basic, Digest, Bearer, API Keys, HMAC y AWS SigV4.
- [`02-session-based/`](./02-session-based/) — **Session-Based Auth** (3 métodos): Autenticación basada en sesión del lado del servidor: cookies de sesión, cookies firmadas y sticky sessions.
- [`03-token-based/`](./03-token-based/) — **Token-Based Auth** (5 métodos): Tokens autocontenidos y por referencia: JWT, PASETO, tokens opacos con introspección, refresh tokens y DPoP.
- [`04-oauth-oidc/`](./04-oauth-oidc/) — **OAuth 2.x / OIDC** (10 métodos): El ecosistema OAuth 2.0/2.1 y OpenID Connect: flujos estándar, PKCE, device flow, token exchange y FAPI 2.
- [`05-sso-federation/`](./05-sso-federation/) — **SSO & Federation** (5 métodos): Single Sign-On y federación de identidad: SAML 2, WS-Federation, CAS, SCIM 2 y social login.
- [`06-directory-services/`](./06-directory-services/) — **Directory Services** (4 métodos): Autenticación contra directorios: LDAP/LDAPS, Active Directory, Kerberos y NTLMv2.
- [`07-network-aaa/`](./07-network-aaa/) — **Network AAA** (12 métodos): Authentication, Authorization & Accounting en redes: 802.1X, variantes EAP, RADIUS, TACACS+ y Diameter.
- [`08-passwordless-fido/`](./08-passwordless-fido/) — **Passwordless & FIDO** (8 métodos): Autenticación sin contraseña: FIDO2/WebAuthn, CTAP2, Passkeys (sincronizadas y device-bound), CXP/CXF, magic links y OTPs.
- [`09-mfa-2fa/`](./09-mfa-2fa/) — **MFA / 2FA** (5 métodos): Autenticación de múltiples factores: TOTP, HOTP, push con number matching, hardware tokens y backup codes.
- [`10-biometrics/`](./10-biometrics/) — **Biometrics** (4 métodos): Autenticación biométrica local: Touch ID, Face ID, Windows Hello y biometría conductual.
- [`11-pki-mtls/`](./11-pki-mtls/) — **PKI & mTLS** (5 métodos): Infraestructura de clave pública: certificados X.509 de cliente, mTLS, SSH keys/certs y SPIFFE/SPIRE.
- [`12-pake-crypto/`](./12-pake-crypto/) — **PAKE & Crypto Auth** (3 métodos): Password-Authenticated Key Exchange criptográfico: SRP, SCRAM y OPAQUE.
- [`13-decentralized-web3/`](./13-decentralized-web3/) — **Decentralized & Web3** (3 métodos): Identidad descentralizada: Sign-In with Ethereum, DIDs y Verifiable Credentials.
- [`14-workload-cloud-identity/`](./14-workload-cloud-identity/) — **Workload & Cloud Identity** (5 métodos): Identidad de workloads en la nube: AWS IAM Roles, GCP WIF, Azure Managed Identities, K8s ServiceAccount tokens y OIDC federation para CI/CD.
- [`15-agent-identity/`](./15-agent-identity/) — **Agent Identity** (6 métodos): Identidad para agentes de IA: OAuth 2.1 para MCP, Agentic JWT, AIMS/WIMSE, delegation tokens/macaroons, signed agent cards y AP2.
- [`16-zero-trust-continuous/`](./16-zero-trust-continuous/) — **Zero Trust & Continuous Auth** (5 métodos): Autenticación continua y zero trust: CAEP, SSF, auth adaptativa, device posture y acceso condicional.

---

## Tabla comparativa

| Método | Categoría | Estado | Factor (sé/tengo/soy) | Phishing-resistant | Transporte | Caso de uso típico |
|--------|-----------|--------|----------------------|--------------------|------------|-------------------|
<!-- Completar a medida que se estudian los métodos -->

---

## Progreso

### 01-http-auth-basics — HTTP Auth Basics

- [ ] 🟢 Vigente [Basic Auth](./01-http-auth-basics/01-basic-auth/)
- [ ] 🟡 Legacy pero en uso [Digest Auth](./01-http-auth-basics/02-digest-auth/)
- [ ] 🟢 Vigente [Bearer Token](./01-http-auth-basics/03-bearer-token/)
- [ ] 🟢 Vigente [API Keys](./01-http-auth-basics/04-api-keys/)
- [ ] 🟢 Vigente [HMAC Request Signing](./01-http-auth-basics/05-hmac-request-signing/)
- [ ] 🟢 Vigente [AWS Signature Version 4 (SigV4)](./01-http-auth-basics/06-aws-sigv4/)

### 02-session-based — Session-Based Auth

- [ ] 🟢 Vigente [Session Cookies](./02-session-based/01-session-cookies/)
- [ ] 🟢 Vigente [Signed Cookies](./02-session-based/02-signed-cookies/)
- [ ] 🟡 Legacy pero en uso [Sticky Sessions](./02-session-based/03-sticky-sessions/)

### 03-token-based — Token-Based Auth

- [ ] 🟢 Vigente [JWT (JSON Web Token)](./03-token-based/01-jwt/)
- [ ] 🟢 Vigente [PASETO](./03-token-based/02-paseto/)
- [ ] 🟢 Vigente [Opaque Tokens + Introspection](./03-token-based/03-opaque-tokens-introspection/)
- [ ] 🟢 Vigente [Refresh Tokens & Rotation](./03-token-based/04-refresh-tokens-rotation/)
- [ ] 🔵 Emergente / Nuevo 2025-2026 [DPoP (Demonstrating Proof of Possession)](./03-token-based/05-dpop/)

### 04-oauth-oidc — OAuth 2.x / OIDC

- [ ] 🟢 Vigente [OAuth 2.0 — Authorization Code](./04-oauth-oidc/01-oauth2-authorization-code/)
- [ ] 🟢 Vigente [OAuth 2.0 — Client Credentials](./04-oauth-oidc/02-oauth2-client-credentials/)
- [ ] 🟡 Legacy pero en uso [OAuth 2.0 — Implicit Flow](./04-oauth-oidc/03-oauth2-implicit/)
- [ ] 🟡 Legacy pero en uso [OAuth 2.0 — Password Grant](./04-oauth-oidc/04-oauth2-password-grant/)
- [ ] 🟢 Vigente [OAuth 2.0 — Device Flow](./04-oauth-oidc/05-oauth2-device-flow/)
- [ ] 🟢 Vigente [PKCE (Proof Key for Code Exchange)](./04-oauth-oidc/06-pkce/)
- [ ] 🔵 Emergente / Nuevo 2025-2026 [OAuth 2.1](./04-oauth-oidc/07-oauth21/)
- [ ] 🟢 Vigente [OpenID Connect (OIDC)](./04-oauth-oidc/08-openid-connect/)
- [ ] 🟢 Vigente [Token Exchange (RFC 8693)](./04-oauth-oidc/09-token-exchange/)
- [ ] 🔵 Emergente / Nuevo 2025-2026 [FAPI 2.0 (Financial-grade API)](./04-oauth-oidc/10-fapi-2/)

### 05-sso-federation — SSO & Federation

- [ ] 🟢 Vigente [SAML 2.0](./05-sso-federation/01-saml2/)
- [ ] 🟡 Legacy pero en uso [WS-Federation](./05-sso-federation/02-ws-federation/)
- [ ] 🟡 Legacy pero en uso [CAS (Central Authentication Service)](./05-sso-federation/03-cas/)
- [ ] 🟢 Vigente [SCIM 2.0](./05-sso-federation/04-scim2/)
- [ ] 🟢 Vigente [Social Login (OAuth-based)](./05-sso-federation/05-social-login/)

### 06-directory-services — Directory Services

- [ ] 🟢 Vigente [LDAP / LDAPS](./06-directory-services/01-ldap-ldaps/)
- [ ] 🟢 Vigente [Active Directory Bind](./06-directory-services/02-active-directory-bind/)
- [ ] 🟢 Vigente [Kerberos](./06-directory-services/03-kerberos/)
- [ ] 🟡 Legacy pero en uso [NTLMv2](./06-directory-services/04-ntlmv2/)

### 07-network-aaa — Network AAA

- [ ] 🟢 Vigente [802.1X](./07-network-aaa/01-8021x/)
- [ ] 🟢 Vigente [EAP-TLS](./07-network-aaa/02-eap-tls/)
- [ ] 🟢 Vigente [EAP-TTLS](./07-network-aaa/03-eap-ttls/)
- [ ] 🟢 Vigente [EAP-PEAP](./07-network-aaa/04-eap-peap/)
- [ ] 🟡 Legacy pero en uso [EAP-FAST](./07-network-aaa/05-eap-fast/)
- [ ] 🟡 Legacy pero en uso [EAP-MD5](./07-network-aaa/06-eap-md5/)
- [ ] 🟢 Vigente [EAP-SIM / EAP-AKA](./07-network-aaa/07-eap-sim-aka/)
- [ ] 🟢 Vigente [RADIUS](./07-network-aaa/08-radius/)
- [ ] 🟢 Vigente [TACACS+](./07-network-aaa/09-tacacs-plus/)
- [ ] 🟢 Vigente [Diameter](./07-network-aaa/10-diameter/)
- [ ] 🟡 Legacy pero en uso [PAP (Password Authentication Protocol)](./07-network-aaa/11-pap/)
- [ ] 🟡 Legacy pero en uso [CHAP / MS-CHAPv2](./07-network-aaa/12-chap-mschapv2/)

### 08-passwordless-fido — Passwordless & FIDO

- [ ] 🟢 Vigente [FIDO2 / WebAuthn](./08-passwordless-fido/01-fido2-webauthn/)
- [ ] 🟢 Vigente [CTAP2 (Client to Authenticator Protocol 2)](./08-passwordless-fido/02-ctap2/)
- [ ] 🔵 Emergente / Nuevo 2025-2026 [Passkeys — Synced](./08-passwordless-fido/03-passkeys-synced/)
- [ ] 🔵 Emergente / Nuevo 2025-2026 [Passkeys — Device-Bound](./08-passwordless-fido/04-passkeys-device-bound/)
- [ ] 🔵 Emergente / Nuevo 2025-2026 [CXP / CXF (Credential Exchange)](./08-passwordless-fido/05-cxp-cxf/)
- [ ] 🟢 Vigente [Magic Links](./08-passwordless-fido/06-magic-links/)
- [ ] 🟢 Vigente [Email OTP](./08-passwordless-fido/07-email-otp/)
- [ ] 🟡 Legacy pero en uso [SMS OTP](./08-passwordless-fido/08-sms-otp/)

### 09-mfa-2fa — MFA / 2FA

- [ ] 🟢 Vigente [TOTP (Time-based OTP)](./09-mfa-2fa/01-totp/)
- [ ] 🟢 Vigente [HOTP (HMAC-based OTP)](./09-mfa-2fa/02-hotp/)
- [ ] 🟢 Vigente [Push + Number Matching](./09-mfa-2fa/03-push-number-matching/)
- [ ] 🟢 Vigente [Hardware Tokens (YubiKey, etc.)](./09-mfa-2fa/04-hardware-tokens/)
- [ ] 🟢 Vigente [Backup Codes](./09-mfa-2fa/05-backup-codes/)

### 10-biometrics — Biometrics

- [ ] 🟢 Vigente [Touch ID / Fingerprint](./10-biometrics/01-touch-id-fingerprint/)
- [ ] 🟢 Vigente [Face ID](./10-biometrics/02-face-id/)
- [ ] 🟢 Vigente [Windows Hello](./10-biometrics/03-windows-hello/)
- [ ] 🔵 Emergente / Nuevo 2025-2026 [Behavioral Biometrics](./10-biometrics/04-behavioral-biometrics/)

### 11-pki-mtls — PKI & mTLS

- [ ] 🟢 Vigente [X.509 Client Certificates](./11-pki-mtls/01-x509-client-certs/)
- [ ] 🟢 Vigente [mTLS (Mutual TLS)](./11-pki-mtls/02-mtls/)
- [ ] 🟢 Vigente [SSH Keys](./11-pki-mtls/03-ssh-keys/)
- [ ] 🟢 Vigente [SSH Certificates](./11-pki-mtls/04-ssh-certificates/)
- [ ] 🔵 Emergente / Nuevo 2025-2026 [SPIFFE / SPIRE](./11-pki-mtls/05-spiffe-spire/)

### 12-pake-crypto — PAKE & Crypto Auth

- [ ] 🟢 Vigente [SRP (Secure Remote Password)](./12-pake-crypto/01-srp/)
- [ ] 🟢 Vigente [SCRAM (Salted Challenge Response Auth. Mechanism)](./12-pake-crypto/02-scram/)
- [ ] 🔵 Emergente / Nuevo 2025-2026 [OPAQUE](./12-pake-crypto/03-opaque/)

### 13-decentralized-web3 — Decentralized & Web3

- [ ] 🟢 Vigente [SIWE (Sign-In with Ethereum)](./13-decentralized-web3/01-siwe/)
- [ ] 🔵 Emergente / Nuevo 2025-2026 [DIDs (Decentralized Identifiers)](./13-decentralized-web3/02-dids/)
- [ ] 🔵 Emergente / Nuevo 2025-2026 [Verifiable Credentials (VC)](./13-decentralized-web3/03-verifiable-credentials/)

### 14-workload-cloud-identity — Workload & Cloud Identity

- [ ] 🟢 Vigente [AWS IAM Roles](./14-workload-cloud-identity/01-aws-iam-roles/)
- [ ] 🟢 Vigente [GCP Workload Identity Federation](./14-workload-cloud-identity/02-gcp-workload-identity-federation/)
- [ ] 🟢 Vigente [Azure Managed Identities](./14-workload-cloud-identity/03-azure-managed-identities/)
- [ ] 🟢 Vigente [Kubernetes ServiceAccount Tokens](./14-workload-cloud-identity/04-k8s-serviceaccount-tokens/)
- [ ] 🟢 Vigente [OIDC Federation — GitHub Actions](./14-workload-cloud-identity/05-oidc-federation-github-actions/)

### 15-agent-identity — Agent Identity

- [ ] 🔵 Emergente / Nuevo 2025-2026 [OAuth 2.1 for MCP](./15-agent-identity/01-oauth21-for-mcp/)
- [ ] 🔵 Emergente / Nuevo 2025-2026 [Agentic JWT](./15-agent-identity/02-agentic-jwt/)
- [ ] 🔵 Emergente / Nuevo 2025-2026 [AIMS / WIMSE](./15-agent-identity/03-aims-wimse/)
- [ ] 🔵 Emergente / Nuevo 2025-2026 [Delegation Tokens & Macaroons](./15-agent-identity/04-delegation-tokens-macaroons/)
- [ ] 🔵 Emergente / Nuevo 2025-2026 [Signed Agent Cards (A2A)](./15-agent-identity/05-signed-agent-cards-a2a/)
- [ ] 🔵 Emergente / Nuevo 2025-2026 [AP2 — Agent Payments Protocol](./15-agent-identity/06-ap2-agent-payments/)

### 16-zero-trust-continuous — Zero Trust & Continuous Auth

- [ ] 🔵 Emergente / Nuevo 2025-2026 [CAEP (Continuous Access Evaluation Protocol)](./16-zero-trust-continuous/01-caep/)
- [ ] 🔵 Emergente / Nuevo 2025-2026 [Shared Signals Framework (SSF)](./16-zero-trust-continuous/02-shared-signals-framework/)
- [ ] 🟢 Vigente [Risk-Based / Adaptive Auth](./16-zero-trust-continuous/03-risk-based-adaptive-auth/)
- [ ] 🟢 Vigente [Device Posture](./16-zero-trust-continuous/04-device-posture/)
- [ ] 🟢 Vigente [Conditional Access](./16-zero-trust-continuous/05-conditional-access/)

---

## Roadmap sugerido (6 meses, 3-4 métodos por semana)

| Semanas | Categorías | Tema |
|---------|------------|------|
| 1–2   | 01 + 03      | HTTP basics + tokens — fundamentos |
| 3–6   | 04           | OAuth 2.x / OIDC — donde vive el 80 % del auth moderno |
| 7–8   | 05 + 06      | SSO + directorios |
| 9–12  | 08 + 09      | Passwordless/FIDO + MFA |
| 13–16 | 07           | Network AAA |
| 17–20 | 11 + 14 + 16 | PKI, workload identity, zero trust |
| 21–24 | 12 + 13 + 15 | PAKE, Web3, Agent identity |
| Intercaladas | 02 + 10 | Session-based + biometrics (donde encajen) |
