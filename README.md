# mu-cloudfront
Extension to create a CloudFront distribution in front of the ALB for a mu environment.  
Additionally:
* It will create an S3 bucket for static resources.
* It will block all incoming traffic other than CloudFront from ALB 

Sample usage: 

```
## Specify the id of an ACM cert for CloudFront to use (must be in us-east-1)
parameters:
  mu-loadbalancer-acceptance:
    CloudFrontCert: "0000000-0000-0000-0000-000000000"
    CloudFrontDns: "your domain"

extensions:
- url: https://github.com/wisdo/mu-cloudfront/archive/v1.0.zip
```



