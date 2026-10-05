# Awesome-Key-Secrets-Management

## Top Key & Secrets Management Platforms Ecosystem

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

> **Market Overview:** The Secrets Management Solutions market is estimated at **~$4.22 Billion in 2025/2026** (projected to reach **~$8.05 Billion by 2030**). The sector is **moderately to highly fragmented**, characterized by competition between hyperscale cloud-native vaults (AWS, Azure, GCP), traditional security/identity giants (Palo Alto Networks / CyberArk, IBM / HashiCorp), and specialized developer-first secrets platforms (1Password, Bitwarden, Akeyless, Doppler, Infisical).

| Product / Platform | Company Size (Revenue / Valuation) | Starting Price | Free Tier / Trial Limits |
| :--- | :--- | :--- | :--- |
| **[Azure Key Vault](https://azure.microsoft.com/products/key-vault/)**<br>Microsoft's managed vault for secrets, keys, and certificates with native Azure IAM integration. | ~$3.10T Market Cap<br>(~$245B Annual Revenue) | $0.03 per 10,000 secret operations; HSM keys from $1.00/key/month | Azure Free Account provides $200 credit (valid 30 days) + 10,000 free operations/month for standard secrets |
| **[Google Cloud Secret Manager](https://cloud.google.com/secret-manager)**<br>Google Cloud's managed secrets store with versioning and IAM access controls across GCP services. | ~$2.10T Market Cap<br>(~$307B Annual Revenue) | $0.06 per active secret version/month + $0.03 per 10,000 API operations | Always Free tier includes 6 active secret versions & 10,000 access operations free per month |
| **[AWS Secrets Manager](https://aws.amazon.com/secrets-manager/)**<br>Fully managed AWS service for storing and rotating database credentials and API keys with native IAM integration. | ~$2.00T Market Cap<br>(~$575B Revenue / AWS ~$100B+) | $0.40 per secret stored/month + $0.05 per 10,000 API calls | 30-day free trial with 10 secrets & 10,000 API calls; new AWS accounts receive $200 in free credits |
| **[HashiCorp Vault (HCP Vault)](https://www.hashicorp.com/products/vault)**<br>Enterprise secrets management platform offering dynamic credentials, encryption as a service, and PKI. | ~$200B Market Cap (IBM)<br>(Acquired HashiCorp for $6.4B) | HCP Vault Radar starts at $0.25/secret/month; HCP Vault Dedicated from $0.03/hour (~$22/month) | $50 in free credits valid for 30 days on HCP Vault Cloud; self-hosted Open Source edition free forever |
| **[CyberArk Conjur](https://www.cyberark.com/products/privileged-access-management/conjur/)**<br>Enterprise secrets management focused on privileged access management (PAM) and machine identities. | ~$110B Market Cap (Palo Alto Networks)<br>(Acquired CyberArk for $25B; $1.36B Rev) | Enterprise SaaS platform starts at ~$15,000/year base licensing | 30-day free trial for Cloud SaaS; open-source core (Conjur OSS) free forever for self-hosting |
| **[1Password Secrets Automation](https://1password.com/developers/secrets-automation)**<br>Developer secrets automation integrating password management with machine secrets, service accounts, and CI/CD pipelines. | $6.80B Valuation<br>(~$400M+ ARR) | Included in Business plan at $7.99/user/month (includes 3 service accounts & 50 secrets; extra secrets $1/month) | 14-day free trial with full feature access (up to 100 secrets/users during trial); no perpetual free tier |
| **[Bitwarden Secrets Manager](https://bitwarden.com/products/secrets-manager/)**<br>DevOps secrets management solution integrated into the broader Bitwarden open-source security ecosystem. | ~$500M - $1.00B Valuation<br>($100M VC Raised) | Teams plan starts at $6.00/user/month (includes 50 secrets & 3 service accounts; additional secrets $0.50/month) | Free forever plan includes up to 2 users, 3 projects, 3 machine accounts, and 50 secrets |
| **[Akeyless](https://www.akeyless.io/)**<br>SaaS-delivered secrets management platform using distributed Fragment Cryptography (DFC) for zero-trust vaulting. | ~$300M - $400M Valuation<br>($80M VC Raised, ~$17.7M ARR) | Starter Enterprise plan starts at $250/month (includes 500 static secrets & 5 client connections) | Free plan includes 5 clients, 500 static secrets, 5 dynamic secrets, and 1 certificate issuer forever |
| **[Doppler](https://www.doppler.com/)**<br>Developer-centric secret management platform focused on environment variable sync, secret injection, and multi-cloud CI/CD pipelines. | ~$100M Valuation<br>($20M VC Raised) | Team plan starts at $7.00/user/month; Enterprise plan at $18.00/user/month | Developer plan is free forever for up to 5 users, unlimited secrets, and 3 environments |
| **[Infisical (Cloud)](https://infisical.com/)**<br>Modern developer-first secrets management platform offering secret sync, secret scanning, PKI, and access control. | ~$50M - $100M Valuation<br>($19M VC Raised, ~$1.7M ARR) | Pro plan starts at $18.00 per identity (user/machine) per month | Free Cloud plan includes up to 5 identities, 3 projects, and 3 environments forever |



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
