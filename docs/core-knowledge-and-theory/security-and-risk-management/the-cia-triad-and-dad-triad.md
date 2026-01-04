# The CIA Triad and DAD Triad

## The CIA Triad: Core Security Objectives

The **CIA Triad** (Confidentiality, Integrity, Availability) represents the three fundamental objectives of information security that every security program aims to achieve.

### Confidentiality

- **Definition:** Ensuring information is accessible only to authorized individuals, systems, or processes. Prevents unauthorized disclosure.
- **Core Question:** "Who should have access to this information?"
- **Example Threats:** Data breaches, eavesdropping, unauthorized access

### Integrity

- **Definition:** Maintaining the accuracy, completeness, and trustworthiness of information throughout its lifecycle. Prevents unauthorized modification.
- **Core Question:** "Can we trust this information hasn't been altered?"
- **Example Threats:** Data tampering, unauthorized changes, malware infection

### Availability

- **Definition:** Ensuring information and systems are accessible and usable by authorized users when needed.
- **Core Question:** "Can authorized users access this when they need it?"
- **Example Threats:** Denial-of-Service attacks, hardware failures, natural disasters

---

**The Balancing Act:** Security professionals must often make trade-offs between these principles. For example:

- Strong encryption (Confidentiality) may impact system performance (Availability)
- Strict change controls (Integrity) might delay critical security patches
- Complex authentication (Confidentiality) could create access barriers during emergencies

---

## The DAD Triad: The Adversarial Perspective

The **DAD Triad** (Disclosure, Alteration, Destruction) represents the inverse of CIA, the primary goals of attackers or negative outcomes of security failures. It's a valuable tool for threat modeling and understanding what you're defending against.

### Direct Correlation: CIA vs. DAD

| CIA Objective (What We Protect) | DAD Failure State (What We Prevent)                             |
| ------------------------------- | --------------------------------------------------------------- |
| **Confidentiality**             | **Disclosure** – Unauthorized exposure of information           |
| **Integrity**                   | **Alteration** – Unauthorized modification or corruption        |
| **Availability**                | **Destruction** – Disruption of access or deletion of resources |

---

## Key Takeaways

1. **CIA is Proactive:** Defines what you're trying to achieve in your security program
2. **DAD is Reactive/Predictive:** Helps anticipate what attackers will try to do
3. **Complementary Models:** Use CIA to set goals, DAD to identify threats
4. **Not Always Equal:** Different assets have different CIA priorities (e.g., public website: Availability > Confidentiality; trade secret: Confidentiality > Availability)
5. **Foundation for Everything:** These concepts underpin all other security domains (access control (CIA), [cryptography](../security-architecture-and-engineering/cryptography.md) (C/I), BCP/DRP (A), etc.)
