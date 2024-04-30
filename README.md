# Data-Governance

Data is one of the most importanat resources an organization possesses in todays economy.

# WHAT IS DATA GOVERNANCE

* Data governance is a set of rules and procedures to manage an organization's data. It ensures data is accurate, secure, and usable for various purposes.
* Similar to how governments create laws, organizations set data policies to define how data is used, accessed, and protected.
* These policies cover data quality, data attributes, data access permissions, data security, regulations compliance, and data privacy.
* Organizations also implement controls (procedures and technology) to enforce these data governance standards.
* Successful data governance requires strong support from executives across the organization, not just the IT department.

# Data Governance Roles

* Data Stewardship: Overseeing data quality, security, privacy, and regulation compliance.
Organizational Data Steward: Leads data governance activities and connects technical and non-technical teams.
Works with Data Owners (senior leaders responsible for specific data areas) to define policies.
May delegate tasks to Subject Area Data Stewards (understand nuances of their specific data domain)

* Data Owners: Senior leaders responsible for a specific data domain (e.g., finance, HR).

* Data Custodians: (Often IT staff) implement technical controls to enforce data governance policies (e.g., configuring access controls).

# Collaboration is Key

The organizational data steward works with all these roles to ensure proper data governance:

* Vertically (across different levels) with data owners and subject area data stewards.
* Horizontally with data custodians responsible for implementing technical controls.
  
# Data Access Requirements

* Access to data is granted based on specific needs.
* Access level varies by data domain and can be limited to specific data fields.
* Example: Managers need access to employee names, contact info, and performance data, but not Social Security numbers.

# organizational example 

![image](https://github.com/SesethuPotye/Data-Governance/assets/162969678/9b1f47c7-5ea0-46d6-9aa5-6678530fb286)

# Determining access requirements
it is essential to develop a data classification matrix. A data classification matrix defines categories, and disclosure implications for data.

# Table showing ana example of data classification.
![image](https://github.com/SesethuPotye/Data-Governance/assets/162969678/555f37f7-455d-4f74-bf15-46e7c17be782)

# Access Permissions

It is granting access based on roles simplifies permission management, especially with employee job changes.


Example: Ralph changes roles from Finance to Facilities to HR (Figure 2).
His access is adjusted based on his new role (Finance -> Facilities -> HR).

![image](https://github.com/SesethuPotye/Data-Governance/assets/162969678/a0c0e335-2ca8-41e9-b31f-49a55de31074)

# BENEFITS OF ROLE-BASED ACCESS

* Easier to maintain permissions and ensure consistency.
* Users only have access to data required for their current role (data security).
* Simplifies permission audits for compliance.

# RISKS OF USER-BASED ACCESS

* Assigning permissions directly to users is risky and complex.
* Increases chance of errors, like forgetting to remove old permissions (Figure 3).
* Can lead to users having too much access (security risk).


![image](https://github.com/SesethuPotye/Data-Governance/assets/162969678/664f41ea-3cbe-465e-8766-a658da85908d)

# Group Permissions

When developing a role-based access strategy, it is common to implement user group-based permissions.

EXAMPLE OF SAMPLE ORGANIZATION CHART

![image](https://github.com/SesethuPotye/Data-Governance/assets/162969678/fcf79a65-61f6-4560-ad05-18a4aa9d4fae)

# Data Use Agreements

A Data Use Agreement (DUA) is a contract between organizations that outlines the rules for sharing private data.  It's important to have a DUA in place before you give any private data to another organization. When creating a DUA, you need to consider how sensitive the data is. The more sensitive the data, the stricter the rules in the DUA should be about how it can be shared.

# example of group based roles
![image](https://github.com/SesethuPotye/Data-Governance/assets/162969678/87f2c7a2-6ad4-4320-b610-363270393377)


# DUA: Rules for Sharing Private Data

* A DUA is a contract that sets the rules for securely transferring, using, and disclosing private data between organizations.
* It specifies details like:
  * Who receives the data
  * How the data can be used (restrictions may apply)
  * How the data is transferred
  * How the recipient protects the data
  * No further distribution of the data without permission
* DUA approval processes vary by organization.
* Legal and regulatory requirements may influence the process.
In the US:
IRB approval needed for research on human subjects (FDA)
HIPAA compliance required for sharing protected health information


# Security Requirements


* Encryption scrambles data using a key, making it unreadable without the key. This protects data at rest (stored) and in transit (moving).
* Encryption Key: A secret code used for encryption and decryption. Losing the key makes the encrypted data inaccessible.
  
# Securing Data at Rest

* Databases are easier to secure due to centralized storage and access controls.

  * Transparent Data Encryption (TDE) encrypts database files for additional 
   security (e.g., Oracle and Microsoft offer TDE).
* Flat Files (on portable devices) pose a bigger challenge due to the risk of physical loss.

  * Device Encryption protects flat files if the device is lost or stolen (as long 
    as the encryption key is safe
    Securing Data in Transit

* HTTPS (Hypertext Transfer Protocol Secure): Encrypts the connection between two locations transferring data.
  * Combines HTTP (data transfer protocol) with TLS (Transport Layer Security) for encryption.



# EXAMPLE OF ENCRYPTED NETWORK CONNECTION 
![image](https://github.com/SesethuPotye/Data-Governance/assets/162969678/f004d9c0-716a-4195-9172-bfa8e4cdafc8)

When a person navigates the Internet using a web browser, a padlock shows up in the address bar to indicate an encrypted HTTPS connection.

# EXAMPLE OF PADLOCK
![image](https://github.com/SesethuPotye/Data-Governance/assets/162969678/5b2a83fe-e902-426d-84df-56bc681525a5)


ETL processes copy data between transactional and analytical systems. When copying files between the transactional and analytical servers, use the Secure Copy Protocol (SCP) or the Secure File Transfer Protocol (SFTP). As their names imply, both SCP and SFTP establish an encrypted tunnel to copy data

# EXAMPLE OF ETL PROCESS 

![image](https://github.com/SesethuPotye/Data-Governance/assets/162969678/c25ab663-5018-433f-8dc1-a5b66bc14a95)

# Data Masking:

* Data masking replaces sensitive data elements (like Social Security numbers) with fake but realistic data in non-production environments (testing, training).
* This protects real people's privacy and reduces risk for the organization.
* Masking doesn't affect the usefulness of data for testing or training purposes (e.g., using a fake SSN for testing doesn't impact the test)


  # Data masking ETL process
![image](https://github.com/SesethuPotye/Data-Governance/assets/162969678/2bccaa45-2fb4-4926-90b6-8b5a7e4541ab)










































































































