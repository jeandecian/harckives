# Access Control Models

Access control is a **core security principle** that determines who or what can view, use, or modify resources in a system. It ensures that only authorized users and processes have the appropriate level of access. Below are the **primary types of access control models**, each with its own approach to managing permissions.

## Discretionary Access Control (DAC)

- **DAC** allows the **owner** of a resource (e.g., file, folder) to decide who can access it and what permissions they have.
- Access is granted at the discretion of the owner.

### Key Characteristics of DAC

- **Flexible:** Owners can freely grant or revoke access.
- **User-Centric:** Users control access to their own resources.
- **Example:** File permissions in Windows (e.g., sharing a folder with specific users).

## Mandatory Access Control (MAC)

- **MAC** is a **strict, policy-driven** model where access is determined by a **central authority** (e.g., system administrator or security policy).
- Users and processes cannot change access permissions.

### Key Characteristics of MAC

- **Rule-Based:** Access is granted based on predefined rules (e.g., security clearance levels).
- **Hierarchical:** Uses labels (e.g., "Top Secret," "Confidential") to classify resources and users.
- **Example:** Military or government systems (e.g., Bell-LaPadula model).

## Role-Based Access Control (RBAC)

- **RBAC** grants access based on **user roles** (e.g., "Admin," "Editor," "Viewer").
- Permissions are assigned to roles, and users inherit permissions based on their role.

### Key Characteristics of RBAC

- **Scalable:** Simplifies permission management in large organizations.
- **Role Assignment:** Users are assigned roles, not individual permissions.
- **Example:** Enterprise systems (e.g., Active Directory, AWS IAM).

## Attribute-Based Access Control (ABAC)

- **ABAC** grants access based on **attributes** (e.g., user attributes, resource attributes, environmental conditions).
- Uses policies like "If (user.department = 'Finance' AND resource.type = 'Budget'), then grant access."

### Key Characteristics of ABAC

- **Dynamic:** Access decisions are context-aware.
- **Fine-Grained:** Allows for highly specific access rules.
- **Example:** Modern cloud services (e.g., AWS IAM policies).

## Rule-Based Access Control (RuBAC)

- **RuBAC** grants access based on **predefined rules** (e.g., time of day, location).
- Similar to MAC but often used for specific scenarios (e.g., "Allow access only during business hours").

### Key Characteristics of RuBAC

- **Conditional:** Access is granted based on rules.
- **Example:** Firewall rules, network access control lists (ACLs).

## Choosing the Right Model

- **For simplicity:** Use DAC or RuBAC.
- **For scalability:** Use RBAC.
- **For granularity:** Use ABAC.
- **For high security:** Use MAC.
