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
