# Awesome-Key-Secrets-Management

# Top Key & Secrets Management Platforms Ecosystem
**Curated List of SaaS Products & Open-Source GitHub Projects**
*Focused on Secrets Storage, Dynamic Credentials, Encryption as a Service, Certificate Management & Secure Configuration*
**Last updated: October 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **Key & Secrets Management**. These systems securely store, rotate, inject, and audit secrets (API keys, database credentials, certificates, tokens) across applications, CI/CD, Kubernetes, and multi-cloud environments.

**Examples** include Azure Key Vault, HashiCorp Vault, AWS Secrets Manager, Google Cloud Secret Manager, 1Password Secrets Automation, CyberArk Conjur, Doppler, Infisical, Akeyless, and Bitwarden Secrets Manager (the category leaders).

**Open-source emphasis**: The secrets management space has strong open-source options. **HashiCorp Vault** (community edition), its Linux Foundation fork **OpenBao**, **Infisical**, **CyberArk Conjur**, **SOPS**, and **Bitwarden** provide robust self-hosted alternatives. This section is heavily expanded.

Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saas-products)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms
- **[Azure Key Vault](https://azure.microsoft.com/products/key-vault/)**  
  Microsoft’s managed service for storing secrets, keys, and certificates with tight integration into Azure identity and applications.

- **[HashiCorp Vault (HCP Vault / Enterprise)](https://www.hashicorp.com/products/vault)**  
  Industry-standard secrets management platform offering dynamic secrets, encryption as a service, PKI, and identity-based access (community edition available open-source; enterprise and HCP are commercial).

- **[AWS Secrets Manager](https://aws.amazon.com/secrets-manager/)**  
  Fully managed AWS service for storing and rotating secrets with native IAM integration and automatic rotation for supported services.

- **[Google Cloud Secret Manager](https://cloud.google.com/secret-manager)**  
  Google Cloud’s managed secrets store with versioning, IAM controls, and integration across GCP services.

- **[1Password Secrets Automation](https://1password.com/developers/secrets-automation)**  
  Developer-focused secrets automation from 1Password, combining human password management with machine secrets and CLI/CI integrations.

- **[CyberArk Conjur](https://www.cyberark.com/products/privileged-access-management/conjur/)**  
  Enterprise secrets management solution (open-source core available) focused on privileged access and machine identity in hybrid environments.

- **[Doppler](https://www.doppler.com/)**  
  Developer-friendly secrets platform specialized in environment variable management, sync, and injection across apps and CI/CD.

- **[Infisical (Cloud)](https://infisical.com/)**  
  Modern secrets platform with strong developer experience; offers both open-source self-hosted and commercial cloud editions.

- **[Akeyless](https://www.akeyless.io/)**  
  SaaS secrets management focused on zero-trust, SaaS-delivered vaulting, and dynamic secrets without managing infrastructure.

- **[Bitwarden Secrets Manager](https://bitwarden.com/products/secrets-manager/)**  
  Secrets management offering from Bitwarden, available as part of their broader open-source password and secrets ecosystem.

## Open-Source GitHub Projects
- **[HashiCorp Vault (Community / Open Source)](https://github.com/hashicorp/vault)**  
  The foundational open-source secrets management engine supporting dynamic secrets, transit encryption, PKI, and extensive auth methods (note licensing changes; many teams also evaluate OpenBao).

- **[OpenBao](https://github.com/openbao/openbao)**  
  Linux Foundation fork of Vault under MPL-2.0, providing a fully open-source alternative focused on secrets, dynamic credentials, and encryption as a service.

- **[Infisical](https://github.com/Infisical/infisical)**  
  Open-source secrets, certificates, and privileged access platform with excellent developer UX, secret sync, and self-hosting support (MIT-licensed core).

- **[CyberArk Conjur (Open Source)](https://github.com/cyberark/conjur)**  
  Open-source secrets management and machine identity solution designed for modern DevOps and Kubernetes environments.

- **[Bitwarden](https://github.com/bitwarden)**  
  Open-source password and secrets management ecosystem; Secrets Manager components support machine secrets alongside human credentials.

- **[SOPS (Secrets OPerationS)](https://github.com/getsops/sops)**  
  Mozilla’s open-source tool for encrypting secrets in configuration files (YAML, JSON, ENV) using age, PGP, or cloud KMS—ideal for GitOps workflows.

- **[Mozilla sops + age / age-plugin ecosystems](https://github.com/FiloSottile/age)**  
  Modern encryption primitives commonly paired with SOPS for simple, auditable secret encryption.

- **[Documentation and Vault / OpenBao / Infisical deployment guides](https://developer.hashicorp.com/vault)**  
  Resources for running production secrets systems, configuring auth methods, and integrating with Kubernetes and CI.

- **[Kubernetes External Secrets / Secrets Store CSI drivers](https://github.com/external-secrets/external-secrets)**  
  Open operators that sync secrets from external vaults into Kubernetes secrets.

- **[Berglas / similar cloud-native secret helpers](https://github.com/GoogleCloudPlatform/berglas)**  
  Lightweight tools for managing secrets on specific clouds with encryption at rest.

### Additional Strong Open-Source Options
- Running **OpenBao** or Vault community for full-featured dynamic secrets and encryption-as-a-service.
- Choosing **Infisical** for a modern, developer-centric open-source secrets platform.
- Using **SOPS + age** for GitOps-friendly encrypted configuration.
- Deploying **Conjur** for machine identity and secrets in regulated or Kubernetes-heavy environments.
- Accepting that fully managed cloud services (Azure Key Vault, AWS Secrets Manager, Google Secret Manager) and polished SaaS experiences (Doppler, Akeyless, 1Password Secrets Automation) remain popular for operational simplicity.
- Focusing open-source efforts on control, auditability, multi-cloud flexibility, and avoiding vendor lock-in.

**Frameworks for building custom systems**: Deploy OpenBao or Infisical → configure auth (OIDC, Kubernetes, AppRole) → enable dynamic secrets engines → inject via CSI drivers or CI plugins → encrypt config with SOPS. Suitable for platform teams and security-conscious organizations. Many enterprises combine open-source cores with commercial support or cloud-managed services.

## How to Contribute
1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer
- This is a **community-curated** list — not exhaustive and not an endorsement.
- Secrets management is security-critical. Proper hardening, access policies, audit logging, and rotation strategies are essential. Self-hosted solutions require operational expertise. This list is not security architecture advice.

---
**Made for platform engineers, security teams, and open infrastructure advocates.**
Let's keep secrets protected, rotatable, and as open as practical.
