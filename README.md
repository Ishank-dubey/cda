1. DMS - to migrate the data bases to cloud, SMS(Server Migration Service) to migrate VMWare VMs to AWS
2. WAF - Web Application firewall - to prevent cross site scripting etc. at application layer
3. Step Functions - logs info on the micro services
4. Developer tools -
   - Code commit
   - Code build
   - Code Deploy
   - Code pipeline
5. Policy can be attached to a User or Group or Role.
6. IAM can be used for federate a corporate user using SAML
7. Instance Meta Data - AZ can be found
8. One Region has Minimum 2 AZ
9. JSON spec has -- objects, array, number, string
10.STS(Security Token Service)
   - Federation
     - Uses SAML, grants temporary access, SSO,  user dosent need to be an IAM user
     - Federation using Mobile Apps
     - Cross account access
   - Identity Broker(Takes the passcode and username + IAM Policy + Duration and uses LDAP first and then AWS STS)
   - Identity Store
   - Identities
   - The STS returns 5 things 
     - Access Key
     - Access Token
     - Token
     - Duration > Token's lifetime
     - The creds are verified by S3 in IAM
     - SAML helps in authentication with Active Directory

11. Web identity Federation with Mobile Apps
12. IAM is universal
    - When a new user is created an access key ID and a secret key is obtained that is used to make API calls or CLI or SDK
    - What is the name of the service to allow users to use their social media account to gain temporary access to the AWS           platform - Web Identity Federation
    - The API call used to obtain temporary security credentials when authenticating using Web Identity Federation -                 AssumeRoleWithWebIdentity
    - Name of the API call to request temporary security credentials from the AWS platform when federating with Active       Directory - AssumeRoleWithSAML
    -  1)The user navigates to ADFS webserver, 2) The user enter in their single sign on credentials, 3) The user's web                browser receives a SAML assertion from the AD server, 4) The user's browser then posts the SAML assertion to the AWS          SAML end point for SAML and the AssumeRoleWithSAML API request is used to request temporary security credentials. 5)          The user is then able to access the AWS Console.
    - The AWS sign-in endpoint for SAML is https://signin.aws.amazon.com/saml
    - 1) A user authenticates with facebook first. They are then given an ID token by facebook. An API call called.                    AssumeRoleWithWebIdentity is then used in conjunction with the ID token. A user is then granted temporary security            credentials.
13. EC2
    - On Demand(pay by the hour or second for Linux instances)
    - Reserved have a contract period of 1 year or 3 year terms
      - Standard(75% cost saving as compared to on demand)
      - Convertable (54% saving and can be upgraded to same or higher costs)
      - Scheduled RI
    - On Spot for flexible timings 
    - Dedicated hosts - dedicated hardware, good for licencing
14. EC2 Instance types - DR MCGIFT PX    
15. EBS
    - GPIO - general purpose, upto 10,000 IOPS - SSD and bootable
    - Provisioned IOPS - more than 10k - SSD and bootable
    - Throughout optimized- store sequential data and not bootable
    - Cold HDD - lowest costs - file server and not bootable
    - Magnetic Standard - lowest cost EBS volume and is bootable but for infrequent access
   

