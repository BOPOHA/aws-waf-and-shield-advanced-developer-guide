# Document History<a name="doc-history"></a>

| Change | Description | Date | 
| --- |--- |--- |
| [AWS Firewall Manager support for AWS Shield Advanced](https://docs.aws.amazon.com/waf/latest/developerguide/logging.html) | Added support for Shield Advanced to Firewall Manager\. | March 15, 2019 | 
| [Tutorial: Creating Hierarchical Policies](https://docs.aws.amazon.com/waf/latest/developerguide/logging.html) | Added tutorial on creating hierarchical policies in AWS Firewall Manager\. | February 11, 2019 | 
| [Rule\-level control in rule groups](https://docs.aws.amazon.com/waf/latest/developerguide/logging.html) | You can now exclude individual rules from AWS Marketplace rule groups, as well as your own rule groups\. | December 12, 2018 | 
| [AWS Shield Advanced support for AWS Global Accelerator](https://docs.aws.amazon.com/waf/latest/developerguide/logging.html) | Shield Advanced can now protect AWS Global Accelerator\. | November 26, 2018 | 
| [AWS WAF support for Amazon API Gateway](https://docs.aws.amazon.com/waf/latest/developerguide/logging.html) | AWS WAF now protects API Gateway APIs\. | October 25, 2018 | 
| [Expanded AWS Shield Advanced Getting Started wizard](https://docs.aws.amazon.com/waf/latest/developerguide/getting-started-ddos.html) | New wizard provides opportunity to create rate\-based rules and Amazon CloudWatch Events\. | August 31, 2018 | 
| [AWS WAF logging](https://docs.aws.amazon.com/waf/latest/developerguide/logging.html) | Enable logging to get detailed information about traffic that is analyzed by your web ACL\. | August 31, 2018 | 
| [Support for query parameters in conditions](https://docs.aws.amazon.com/waf/latest/developerguide/web-acl-create-condition.html) | When creating a condition, you can now search the requests for specific parameters\. | June 5, 2018 | 
| [Shield Advanced Getting Started Wizard](https://docs.aws.amazon.com/waf/latest/developerguide/getting-started-ddos.html) | Introduces a new streamlined process for subscribing to AWS Shield Advanced\. | June 5, 2018 | 
| [Expanded allowed CIDR ranges](https://docs.aws.amazon.com/waf/latest/developerguide/web-acl-ip-conditions.html) | When creating an IP match condition, AWS WAF now supports IPv4 address ranges: /8 and any range between /16 through /32\.  | June 5, 2018 | 

## Earlier updates<a name="doc-history-early-changes"></a>

The following table describes important changes in each release of the *AWS WAF Developer Guide*\.


| Change | API Version | Description | Release Date | 
| --- | --- | --- | --- | 
| Update | 2016\-08\-24 | Marketplace rule groups | November, 2017 | 
| Update | 2016\-08\-24 | Shield Advanced support for Elastic IP addresses | November, 2017 | 
| Update | 2016\-08\-24 | Global threat environment dashboard | November, 2017 | 
| Update | 2016\-08\-24 | DDoS\-resistant website tutorial | October, 2017 | 
| Update | 2016\-08\-24 | Geo and regex conditions | October, 2017 | 
| Update | 2016\-08\-24 | Rate\-based rules | June, 2017 | 
| Update | 2016\-08\-24 | Reorganization | April, 2017 | 
| Update | 2016\-08\-24 | Added information about DDOS protection and support for Application Load Balancers\. | November, 2016 | 
| Update | 2015\-08\-24 | Added information about [AWS WAF and AWS Shield Advanced PCI DSS Compliance](pci-compliance.md) for AWS WAF\. | July 25, 2016 | 
| New Features | 2015\-08\-24 |  You can now log all your API calls to AWS WAF through AWS CloudTrail, the AWS service that records API calls for your account and delivers log files to your S3 bucket\. CloudTrail logs can be used to enable security analysis, track changes to your AWS resources, and aid in compliance auditing\. Integrating AWS WAF and CloudTrail lets you determine which requests were made to the AWS WAF API, the source IP address from which each request was made, who made the request, when it was made, and more\. If you are already using AWS CloudTrail, you will start seeing AWS WAF API calls in your AWS CloudTrail log\. If you haven't turned on AWS CloudTrail for your account, you can turn on CloudTrail from the [AWS Management Console](https://console.aws.amazon.com/cloudtrail/home)\. There is no additional charge for turning on CloudTrail, but standard rates for Amazon S3 and Amazon SNS usage apply\.  | April 28, 2016 | 
| New Features | 2015\-08\-24 |  You can now use AWS WAF to allow, block, or count web requests that appear to contain malicious scripts, known as cross\-site scripting or XSS\. Attackers sometimes insert malicious scripts into web requests in an effort to exploit vulnerabilities in web applications\. For more information, see [Working with Cross\-site Scripting Match Conditions](web-acl-xss-conditions.md)\.  |  March 29, 2016  | 
| New Features | 2015\-08\-24 |  With this release, AWS WAF adds the following features: [\[See the AWS documentation website for more details\]](http://docs.aws.amazon.com/waf/latest/developerguide/doc-history.html)  |  January 27, 2016  | 
| New Feature | 2015\-08\-24 |  You can now use the AWS WAF console to choose the CloudFront distributions that you want to associate a web ACL with\. For more information, see [Associating or Disassociating a Web ACL and a CloudFront Distribution](https://docs.aws.amazon.com/waf/latest/developerguide/web-acl-working-with.html#web-acl-associating-cloudfront-distribution)\.  |  November 16, 2015  | 
| Initial Release | 2015\-08\-24 |  This is the first release of the *AWS WAF Developer Guide*\.  |  October 6, 2015  | 