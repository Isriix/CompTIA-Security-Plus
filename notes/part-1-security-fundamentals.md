# Part 1 

---

## CIA Triad

| Principle          | Description                                                                  | Example                      |
|-------------------|------------------------------------------------------------------------------|------------------------------|
| Confidentiality    | Ensures information is accessible only to authorised personnel              | Encryption                   |
| Integrity          | Ensures data remains accurate and unaltered                                 | Checksums, hashing           |
| Availability       | Ensures information and resources are accessible when required              | Redundancy, failover systems |

---

## Non-repudiation

Guarantees that an action or event cannot be denied by the parties involved  
Example: digital signatures

---

## CIANA Pentagon

An expansion of the CIA triad that includes:

- Authentication – Verifying identity (e.g. passwords, biometrics)
- Non-repudiation – Assurance of origin or action

---

## The Triple As of Security

| Term             | Description                                                            | Example                  |
|------------------|------------------------------------------------------------------------|--------------------------|
| Authentication   | Verifies the identity of a user or system                              | Username and password    |
| Authorisation    | Determines what an authenticated user is allowed to access or do       | File permissions, roles  |
| Accounting       | Logs and tracks user actions for auditing or usage monitoring          | Event logs, session IDs  |

These principles form the foundation of most cybersecurity frameworks, including Security+, NIST and ISO 27001

---

## Control Categories

| Category         | Examples                                             |
|------------------|------------------------------------------------------|
| Technical         | Operating system controls, firewalls, anti-virus    |
| Managerial        | Administrative controls, policies and procedures    |
| Operational       | Security personnel, awareness programmes, people    |
| Physical          | Locks, badges, fences, access restrictions          |

---

## Control Types

| Type            | Description                                                              |
|------------------|-------------------------------------------------------------------------|
| Preventative     | Blocks access before it occurs                                           |
| Deterrent        | Discourages unwanted behaviour or makes attackers think twice           |
| Detective        | Identifies and alerts on attempted or successful attacks                |
| Corrective       | Responds after an incident to reduce damage and restore operations      |
| Compensating     | Uses alternatives when primary controls are not feasible                |
| Directive        | Provides instruction on expected behaviour                              |

---

## Control Matrix 

| Type           | Technical           | Managerial              | Operational           | Physical                    |
|----------------|---------------------|--------------------------|------------------------|-----------------------------|
| Preventative   | Firewall             | Onboarding policy        | Guard shack            | Door lock                   |
| Deterrent      | Login splash screen  | Threat of demotion       | Reception desk         | Warning sign                |
| Detective      | System logs          | Review of login reports  | Property patrols       | Motion detectors            |
| Corrective     | Backup recovery      | Incident reporting policy| Contacting authorities | Fire extinguisher           |
| Compensating   | Block instead of patch | Separation of duties   | Multiple security staff| Power generator             |
| Directive      | File storage policy  | Compliance enforcement   | Security training      | Authorised personnel only sign |

---

These control types and categories are essential to understanding risk management and layered defence in both Security+ and real-world environments
# Zero Trust Model

The Zero Trust Model operates on the principle that no one should be trusted by default.

To achieve zero trust, two key planes are used: the control plane and the data plane.

---

## Control Plane

The control plane is the overarching framework responsible for defining, managing and enforcing access policies within an organisation. Key elements include:

- **Adaptive Identity**  
  Real-time validation considering the user's behaviour, device, location and more.

- **Threat Scope Reduction**  
  Limits user access to only what is necessary for their work, reducing the network’s potential attack surface and minimising the "blast radius" of any breach.

- **Policy-Driven Access Control**  
  Developing, managing and enforcing user access policies based on roles and responsibilities.

- **Secured Zones**  
  Isolated environments designed to house sensitive data and ensure proper execution of policies.

---


## Data Plane

The data plane consists of components that enforce access decisions and control data flow:

- **Subject/System**  
  The individual or entity attempting to gain access.

- **Policy Engine**  
  Cross-references access requests with predefined policies.

- **Policy Administrator**  
  Establishes and manages access policies.

- **Policy Enforcement Point**  
  Executes the decision to grant or deny access.

---

# Gap Analysis

Gap analysis is the process of evaluating the differences between an organisation’s current performance and its desired performance. It is a valuable tool for improving operations, processes, performance or overall security posture.

Key steps in conducting a gap analysis include:

1. Defining the scope of the analysis.
2. Gathering data on the organisation’s current state.
3. Analysing the data to identify where current performance falls short.
4. Developing a plan to bridge the identified gaps.


---

## Deception Technologies: Honeypots and Related Tools

Honeypots and their variants are designed to **attract, detect and study malicious activity** in a controlled environment without putting production systems at risk.

### Honeypot

A honeypot is a decoy system designed to attract attackers and monitor their activity. It often mimics a vulnerable service or host and helps identify attack patterns and automated tools.

> Typically targets automated or opportunistic attackers, mostly machines (e.g., bots scanning IP ranges).

### Honeynet

A honeynet extends the honeypot concept by using a full network of decoy systems. It presents a more realistic environment for attackers to interact with, allowing deeper analysis of tactics, techniques and procedures (TTPs).

> Built with multiple interconnected honeypots to simulate a full network infrastructure.

### Honey Files

Honey files are **planted documents** containing fake but tempting information—such as `passwords.txt` or `finance_report.xlsx`. These files are monitored so that any unauthorised access triggers alerts.

> Think of them as bait files—opening or copying them triggers alarms, like a digital bear trap.

### Honey Tokens

Honey tokens are **traceable data elements** (e.g., fake credentials, document markers, or embedded tags) placed within a honeypot or legitimate environment. If the token appears elsewhere (e.g., leaked online), it indicates a data breach and possibly reveals the source of the compromise.

> Used to **track malicious actors** and detect leaks by observing the use of unique planted data.

---

> These deception technologies support early detection, attack analysis and intelligence gathering without endangering real assets.


# Change Management

Change management introduces a structured process for applying changes within large or sensitive environments, reducing risks and ensuring continuity.

---

## Why Change Management Matters

- Changes in corporate environments can affect hundreds or thousands of systems.
- Without control, informal updates may break applications or introduce vulnerabilities.
- Formal processes maintain system availability, communicate changes, and prevent errors.

---

## Change Control Process

1. **Request submission**  
   Complete a change control form outlining the reason, scope, timing, and systems affected.

2. **Impact assessment & risk analysis**  
   The change control board evaluates risks (e.g. downtime, business impact) and balances benefits and drawbacks.

3. **Approval or denial**  
   The board decides based on risk vs benefit.

4. **Scheduling**  
   Define exact date/time for implementation, accounting for business cycles and maintenance windows (e.g. off‑hours or weekends).

5. **Implementation & testing**  
   Apply the change in production then verify with the system or application owner. Confirm functionality post‑change.

6. **Backout plan**  
   Always prepare a rollback plan (e.g. uninstall patch or restore from backup) and test it in a sandbox before production deployment.

7. **Review & documentation**  
   Record outcomes, update change logs, and adjust future process iterations.

---

## Key Roles

- **Change requester or owner**  
  Initiates the request, defines scope and liaises with the team.

- **Change control board (CCB)**  
  A group responsible for assessing and approving changes.

- **Stakeholders**  
  Individuals or teams affected by the change (e.g. accounting, shipping, operations).

---

## Considerations

- Evaluate the **risk of not implementing** a change (e.g. leaving vulnerabilities unpatched).
- Schedule changes outside peak periods (e.g. avoid retail holidays, business-critical windows).
- Ensure full **backups** are available before making changes.
- Maintain and improve the change process over time as organisational needs evolve.

---

> Change management is essential in all firms. Documented and enforced policies ensure no-one makes unauthorised changes and that necessary updates occur safely.

# Technical Change Management

### Allow/Deny List.
Allow List - Very restrictive, nothing runs unless it has been approved.

Deny List - Run any application except those on the deny list. 

---

## Purpose and Context

Technical change management ensures changes to production systems (e.g. patches, configuration adjustments, updates) are applied in a controlled manner to reduce risk, downtime and unintended side effects.

---

## Key Process Steps

1. **Pre‑Change Preparation**  
   - Replicate the production environment in a test or sandbox  
   - Perform full backups  
   - Review patch notes or change documentation

2. **Implementation in Test Environment**  
   - Apply updates or configurations first in a non‑production environment  
   - Test thoroughly, verify functionality and performance

3. **Scheduling & Approval**  
   - Plan changes during maintenance windows or offpeak hours  
   - Issue notifications to relevant stakeholders  
   - Confirm approvals from system owners or change control board

4. **Deployment to Production**  
   - Apply change following the tested procedure  
   - Monitor system performance immediately after deployment

5. **Back‑out Plan**  
   - Ensure a rollback plan exists (e.g. uninstall patch, restore backup)  
   - Verify back‑out works in test before deployment

6. **Post‑Change Review**  
   - Confirm the change achieved its intended outcome  
   - Document date, time, results, and any issues encountered  
   - Update configuration management records or CMDB

---

# Public Key Infrastructure (PKI) 

---

## 1. What is PKI?
- **Public Key Infrastructure (PKI)** is an ecosystem of policies, procedures, and systems that manage encryption keys and digital certificates.
- It enables secure electronic transfer of information using:
  - *Asymmetric encryption* (public/private keypairs)
  - *Digital certificates* (binding identities to keys)

---

## 2. Core Components of PKI
1. **Certificate Authority (CA)**
   - Issues and signs digital certificates.
   - Types:
     - *Root CA* – top-level trust anchor.
     - *Intermediate CA* – delegated cert issuers under a root.

2. **Registration Authority (RA)**
   - Acts as verifier of identity before CA issues certs.
   - Receives certificate requests, authenticates, forwards to CA.

3. **Certificate Database & Store**
   - **Database**: internal repository tracking certificate records (issued, revoked).
   - **Certificate Store**: where certificates are installed for use.

4. **Certificate Revocation List (CRL) / OCSP**
   - Lists certificates revoked before expiry.
   - CRL: periodic download.
   - **OCSP**: Online Certificate Status Protocol, real-time status queries.

5. **Key Archival / Recovery**
   - Securely store private keys for:
     - Email encryption recovery.
     - Digital documents signed in the past.

---

## 3. Types of Certificates
- **SSL/TLS certificates** – secure websites.
- **Code signing certificates** – verify software authenticity.
- **Email (S/MIME) certificates** – secure and authenticate email.
- **Client authentication certificates** – authenticate users/devices on networks.

---

## 4. Trust Models
- **Hierarchical Trust Model** (Tree): Root → Intermediate → End-Entity.
- **Mesh/P2P Trust Model**: Certificate exchange among peers.
- **Web of Trust**: users vouch for each other (e.g., PGP).

---

## 5. Asymmetric Encryption Basics
- **Private key**: kept secret.
- **Public key**: freely distributed.
- Data encrypted with a public key can only be decrypted with its private key.
- Signatures: created with private key; verified with public key.

---

## 6. Certificate Lifecycle
1. Key generation (private + public)
2. Certificate signing request (CSR)
3. Identity verification
4. CA issues signed certificate
5. Deployment to users/services
6. Manage revocation (CRL/OCSP)
7. Renewal or deprecation on expiry

---

## 7. Best Practices & Considerations
- Keep your **Root CA offline** and heavily secured.
- Use **Intermediate CAs** for day-to-day issuance.
- Regularly **back up keys** (especially private keys).
- Implement strong **revocation mechanisms**.
- Use secure **cryptographic algorithms**.
- Maintain **certificate transparency and monitoring** to detect misissuance.

---

## 8. Key Use Cases in Enterprises
- Securing websites (HTTPS)
- Email encryption and signing
- Authenticating devices/users
- Signing software code
- Internal VPNs and network segmentation

---

## 9. Table

| Component            | Purpose                                              |
|----------------------|------------------------------------------------------|
| CA / Root CA         | Issue and sign certificates                         |
| RA                   | Validate identities before issuing certs             |
| CRL / OCSP           | Check certificate revocation status                 |
| Cert Database/Store | Keep track and store certificates                    |
| Key Recovery         | Allow retrieval of encrypted data if lost           |

---

