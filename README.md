# Security Presentation

## Kristen
*Security*: The ability to protect information, systems, and assets while delivering business value through risk assessment and mitigation strategies.

**5 key areas** 
- Identity and Access management = who can do what?
- Detection = security events with detective controls
- Infrastructure protection = protecting the system
- Data protection = confidentiality and integrity of data 
- Incident response = responding to security events

![Security Pillar](https://www.playingaws.com/assets/img/posts/2022-05-28-getting-started-with-aws-security/well-architected-tools.png) 

# **IDENTITY AND ACCESS MANAGEMENT (IAM)**
Key to building a secure workload, ensures that only authenticated AND authorized  users/ machines/services are able to access your resources and only in a manner that is intended.

*Signing in : Multifactor on every account,  minimum password length, strong password, avoid resusing passwords.*

**AWS.SSO/Identity and Access Management Center** : Built in or external apps that help manage all access. Why not use single users? Centralized identity provider can create manage and revoke access from a single location.

**AWS Control Tower** : AWS Control Tower is a managed service that provides the easiest way to set up and govern a new, secure, multi-account AWS environment based on best practices established through AWS experience.

**Aws Secrets manager** : Identities with secrets = passwords to database or third party must be stored with automatic rotation, that integrates with amazon RDS. 

**IAM Policies**: Lists of specific granular permissions that govern previously mentioned access including conditions, can apply to user, group, role, or resources.
- *Permissions*: Define access requirements, grant least privilege, use groups to automate instead of individual, limit public and cross account access, reduce permission continuously

LAB EXAMPLE: [JSON documents and how to read them](https://docs.aws.amazon.com/IAM/latest/UserGuide/reference_policies_grammar.html)

- THEY ARE THE WHAT BEHIND THE WHY
![Json example](https://cloudacademy.com/wp-content/uploads/2015/12/Picture17.png)


## Krislim
# **Detection:** 

![Detection](https://image.shutterstock.com/image-vector/ids-intrusion-detection-system-acronym-260nw-1892176897.jpg)

Detection, in other words Intrusion Detection System (IDS) is an application that monitors a network or system and generates an alert when a threat is detected 

  IDS uses two mechanisms to detect attacks

   Anomaly-based detection - The IDS compare the current traffic pattern or system activity against established baselines for any deviation.

   Signature-based detection - The IDS monitors and analyzes the traffic for known patterns of attack.


![Detection](https://th.bing.com/th/id/OIP.Suq6Tnptny7IzX-kQWKFegHaDU?pid=ImgDet&rs=1)


   Two main Intrusion Detection Systems 

   - Network based Intrusion Dectection System (NIDS)

   - Host based Intrusion Detection System (HIDS)
        
      
      


## Nkosi

# **Data Protection:**



![Symmetric Encryption](https://www.cisco.com/c/en/us/products/security/encryption-explained/jcr:content/Grid/category_atl/layout-category-atl/blade_493679486/bladeContents/quarterhalfquarter/QHQ-Half-2/image/image.img.png/1634629737483.png)

**Cryptography** : 
   The discipline that embodies the principles and techniques for providing data
security, including confidentiality and data integrity. 

**Encryption** :  
   The process of using a code , called a cipher, to turn readable data
into unreadable data for another party. 
The cipher contains both algorithims to encrypt and to decrypt the data.

A *key* is a series of numbers and letters that the algorithm uses to encrypt and
decrypt data. Only the owners of the keys can encrypt data.

**Symmetric encryption** uses the same key to encrypt and decrypt the data. The key is a
shared secret between the sender and the receiver. Symmetric encryption is fast and
reliable and is used for bulk data.

**Symmetric encryption** is used for payment applications, to encrypt databases, and to 
verify the identity of the sender of a message in messaging applications.

**Aymmetric encryption** uses both a private key and a public key (a key pair) to encrypt
and decrypt the data. Every user in the conversation has a key pair. Asymmetric
encryption is more complex and much slower than symmetric encryption. However, it
provides more capabilities in the way that keys are managed.

**Asymmetric encryption** is used to encrypt emails or create digital signatures.
(SSH)

**Data in transit** :
   Any data that is sent from one system to another. This includes
communication between resources within your workload as well as communication
between other services and your end users. By providing the appropriate level of
protection for your data in transit, you protect the confidentiality and integrity of your
workload’s data.


## Aissatou 
# **Security: Incident Response**
![Incident Response](https://d2908q01vomqb2.cloudfront.net/22d200f8670dbdb3e253a90eee5098477c95c23d/2022/05/05/Site-Merch_Amazon-GuardDuty_Blog.jpg)

- It's important to have a clear process in place for responding to and minimizing the impact of security incidents. This process should be well-defined and established, so that you can quickly and effectively respond to any security threats that arise.

**Top Recommendation for Incident Response:**

![Incide Response Process](https://uploads-ssl.webflow.com/5fdd14258ef27a3d5aac69fa/61af7f3f99d2799b5db4385d_aws-security-services-incident-response-3.png)

1. Have a plan in place for dealing with security incidents, including detecting, containing, analyzing, and mitigating them.
2. Use AWS monitoring tools like CloudTrail and GuardDuty to identify potential security threats.
3. If a security incident does occur, respond quickly to contain it and minimize the damage.
4. Analyze what happened and figure out what caused the incident so you can prevent it from happening again.
5. Take steps to minimize the impact of the incident and prevent it from happening in the future.
6. Have a clear plan for communicating with anyone who needs to know about the incident.
7. Regularly assess and update your security policies to stay ahead of potential threats.


[**Creating Cloud Trail**](https://drive.google.com/file/d1nOIbfoaWFXYWWxzNKVGn96rdsXT5VRfB/view?usp=sharing)

**Summary:**

![Incident Response Process](https://d1.awsstatic.com/asses-2023/product-rds.5a9aba06b0a59417010ca652cec78591850548be.png)


AWS offers resources and services like AWS Security Hub and AWS Incident Response that can help you respond to security incidents more effectively.


### Additional Notes:

