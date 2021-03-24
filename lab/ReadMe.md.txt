Purpose is:

Single EC2 Running Mediawiki on Nginx, RDS Backed, Behind LB .

Prerequisites:
Create RDS Instance
Create empty Mediawiki Database and User
Internet Access from EC2 Instance

cft Template Details:
EC2 Instance
Amazon Linux
EBS volume
t2.micro (default)
Private Subnet
No External IP
Security Group
Allow 80 Inbound
Allow 443 Inbound
CloudWatch Logs Group
IAM Instance Profile Role
S3 RW Access
Cloudwatch Write Metrics
Cloudwatch Logs
Route 53 Upsert
UserData (Bootstrapping)
Yum Updates
Install minimum packages
cfn-init
aws-cfn-bootstrap
cloud-init
Call cfn-init
