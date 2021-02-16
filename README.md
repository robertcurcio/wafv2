# Stack Description:
Here are 2 CloudFormation stacks specifically for designed to create WebACLs for 1. CloudFront distributions (Global) or 2. For regional use such as ALBs, API Gateway or AppSync 

* Creates a WAFv2 ACL with Amazon managed rules 
* Creates and attaches 2 IP sets (one blacklist and one whitelist)
* The CLOUDFRONT scope must be deployed from us-east-1

Note: In the `Addresses:` list, please add your own custom IPV4 CIDR notations.
