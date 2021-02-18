# Stack Description:
Here are 3 CloudFormation stacks specifically for designed to create WebACLs for WAFv2:

regional-only-webacl.yaml 

* Creates a WAFv2 ACL with Amazon managed rules 
* Creates and attaches 2 IP sets (one blacklist and one whitelist)
* Only works with regions, not Global (No Cloudfront)
* For regional use such as ALBs, API Gateway or AppSync

waf-and-cloudfront.yaml

* Creates a WAFv2 ACL with Amazon managed rules 
* Creates and attaches 2 IP sets (one blacklist and one whitelist)
* This can only be deployed from us-east-1 for the Global
* For use with CloudFront distributions only

waf-with-rulegroup-and-2-ipsets.yaml

* Creates a WAFv2 ACL with Amazon managed rules 
* Creates and attaches 2 IP sets (one blacklist and one whitelist)
* Creates and attaches 1 blank Rule Group
* For use with CloudFront distributions only
