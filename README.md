 Securing Endpoints with BitLocker Drive Encryption

Project Overview

This project documents my real-world experience during my internship, where I deployed BitLocker encryption across organizational devices to protect sensitive data and enforce endpoint security policies.

Objective
To ensure full disk encryption on all eligible workstations, safeguarding data from unauthorized access and theft.

Tools and Technologies Used
- BitLocker Drive Encryption (Windows 10/11)
- Group Policy Editor (GPO)
- Active Directory (for policy management)
- TPM (Trusted Platform Module) for secure encryption key storage

Steps I Took
1. Assessed system compatibility (TPM chip + Windows edition)
2. Enabled BitLocker on domain-joined devices
3. Chose an appropriate encryption method (XTS-AES 256-bit)
4. Backed up recovery keys to Active Directory and cloud
5. Verified encryption status using BitLocker Drive Encryption tool and `manage-bde` command

Outcome
- Achieved full disk encryption across 95%+ of workstations
- Minimized risk of data theft from lost or stolen devices
- Strengthened the organization's endpoint security posture

Skills Demonstrated
- Windows administration & configuration  
- Data protection and encryption protocols  
- Group Policy management  
- Security compliance enforcement  
- Troubleshooting encryption issues (e.g., TPM errors, recovery key loss)

Reflection

What were the risks if encryption wasn’t enabled?
Sensitive company data could be exposed in the event of laptop theft or loss, potentially violating data protection regulations and harming organizational reputation.

What challenges did I face?
Some older systems lacked TPM support, requiring manual configuration or were excluded from encryption. I also had to ensure recovery keys were securely stored and retrievable.

What best practices were followed?
Enforced encryption via Group Policy, used strong AES-XTS 256-bit, ensured recovery keys were backed up securely, and verified status post-deployment.

Notes
This was a foundational experience that introduced me to endpoint protection strategies and gave me hands-on exposure to real-world IT policy enforcement.
