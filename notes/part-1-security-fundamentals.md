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
