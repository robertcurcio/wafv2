# Stack Description:
This is a CloudFormation stack specifically for designed to create WebACLs for CloudFront distributions only: 

* Creates a WAFv2 ACL with Amazon managed rules 
* Creates and attaches 2 IP sets (one blacklist and one whitelist)
* Must be deployed from us-east-1 when scope is CLOUDFRONT

Note: In the `Addresses:` list, please add your own custom IPV4 CIDR notations.
