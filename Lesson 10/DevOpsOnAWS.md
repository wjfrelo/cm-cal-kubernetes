
### #####################
DevOps on AWS [12-June-2021]
### #####################

Free Tier: https://aws.amazon.com/free/

### Global Infrastructure
- Regions | 3 or more availability Zones
- Availability Zones --> Cluster of Data Centres |
- Edge Locations (PoP) --> CDN | Content Delivery Network | Web content caching | 
- AWS backbone network --> High speed low latency cables connecting different AWS DCs across the world

## Regions
  - Default Regions
  - US Gov Cloud
  - China

### Cloud Types
- Public | AWS, Azure, GCP,
- Private | Within Org | Open Stack, Cloud Foundary
- Hybrid | AWS + On prem | Azure + On prem
- Multi | AWS + Azure, AWS + Azure + GCP


### different ways to connect to AWS
  - Console | GUI | User id and Password
  - AWS CLI | command line | Access key id and secret access key
  - SDK | Programmatic access | Access id and secret access key


### Compute on AWS
EC2 --> Xen Server, AWS Nitro Systems
Hypervisors
  - VMware ESXi
  - HyperV
  - RedHat KVM


### Networking on AWS
VPC
  **Routing**  
  - Subnets
  - Route tables
  - Internet Gateway
  - NAT Gateway
  - Virtual Private Gateway
  - ENI (NIC ---> vNIC ---> ENI (Elastic Network Interface))

  **Security**
  - Security Groups
      - Firewall at the instance level
  - NACLs (Network Access control lists)
      - Firewall at the Subnet level

### Types of IP

- Public IP
- Private IP
    - 10.0.0.0
    - 172.31
    - 192.168.0.0

- Dynamic IP --> Public IP
- Static IP --> Elastic IPs

### Storage on AWS (SAN / DAS / NAS)

- Object Storage (C:\mydocuments, D:\mymovies etc. )
    - S3
      - Unlimited data
      - 5TB file size limit
      - Storage classes

- Block Storage (C:\, D:\ etc.)
    - EBS | Persistent Block Storage | SAN
        - SSD Based
        - HDD Based
    - Instance Store | Ephemeral Block Storage | DAS

- File/Network (Network drives like Z:\)
    - EFS | Linux workloads | NFS 4.0 and 4.1
    - FSx | Windows workloads | NTFS, CIFS, SMB,


### EC2 instance Nomenclature

- m5.xlarge
  - m     --> Family
  - 5     --> Generation
  - xlarge --> Size (vCPU / Memory / Network Bandwidth)


### Security on AWS

- IAM (Authentication and Authorization)
    - Users
    - Groups
    - Policies
    - Roles
        - Temporary elevated privileges
        - Federated access
        - Services/application accessing AWS resources
  
- WAF and Shield --> DDoS Mitigation
- Artifact --> For HIPAA/FISMA and other reports
- Inspector --> CVE scanning and reporting

### Compute Evolution

Physical Machines ---> Virtual Machines ---> Containers ---> Serverless


### Further reading
https://docs.aws.amazon.com/cli/latest/userguide/install-cliv2.html
https://aws.amazon.com/tools/
https://aws.amazon.com/getting-started/tools-sdks/
https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/ebs-volume-types.html
https://aws.amazon.com/s3/storage-classes/
https://aws.amazon.com/ec2/instance-types/
https://aws.amazon.com/compliance/
https://aws.amazon.com/compliance/services-in-scope/
https://aws.amazon.com/architecture/security-identity-compliance/
https://aws.amazon.com/compliance/fedramp/
https://d1.awsstatic.com/whitepapers/Security/DDoS_White_Paper.pdf


### Hands-on Labs and Workshops
1. https://ecsworkshop.com/
2. https://eksworkshop.com/
3. https://aws.amazon.com/getting-started/hands-on/
4. https://www.wellarchitectedlabs.com/
5. https://aws-ci-cd.workshop.aws/
6. https://cicd-for-ecs.workshop.aws/en/
7. https://aws.amazon.com/training/ramp-up-guides/












