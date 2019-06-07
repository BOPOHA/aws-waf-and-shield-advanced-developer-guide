# Working with Geographic Match Conditions<a name="web-acl-geo-conditions"></a>

If you want to allow or block web requests based on the country that the requests originate from, create one or more geo match conditions\. A geo match condition lists countries that your requests originate from\. Later in the process, when you create a web ACL, you specify whether to allow or block requests from those countries\.

You can use geo match conditions with other AWS WAF conditions or rules to build sophisticated filtering\. For example, if you want to block certain countries, but still allow specific IP addresses from that country, you could create a rule containing a geo match condition and an IP match condition\. Configure the rule to block requests that originate from that country and do not match the approved IP addresses\. As another example, if you want to prioritize resources for users in a particular country, you could include a geo match condition in two different rate\-based rules\. Set a higher rate limit for users in the preferred country and set a lower rate limit for all other users\.

**Note**  
If you are using the CloudFront geo restriction feature to block a country from accessing your content, any request from that country is blocked and is not forwarded to AWS WAF\. So if you want to allow or block requests based on geography plus other AWS WAF conditions, you should *not* use the CloudFront geo restriction feature\. Instead, you should use an AWS WAF geo match condition\.

**Topics**
+ [Creating a Geo Match Condition](#web-acl-geo-conditions-creating)
+ [Editing Geo Match Conditions](#web-acl-geo-conditions-editing)
+ [Deleting Geo Match Conditions](#web-acl-geo-conditions-deleting)

## Creating a Geo Match Condition<a name="web-acl-geo-conditions-creating"></a>

If you want to allow some web requests and block others based on the countries that the requests originate from, create a geo match condition for the countries that you want to allow and another geo match condition for the countries that you want to block\.

**Note**  
When you add a geo match condition to a rule, you also can configure AWS WAF to allow or block web requests that *do not* originate from the country that you specify in the condition\.<a name="web-acl-geo-conditions-creating-procedure"></a>

**To create a geo match condition**

1. Sign in to the AWS Management Console and open the AWS WAF console at [https://console\.aws\.amazon\.com/waf/](https://console.aws.amazon.com/waf/)\. 

1. In the navigation pane, choose **Geo match**\.

1. Choose **Create condition**\.

1. Type a name in the **Name** field\.

   The name can contain only alphanumeric characters \(A\-Z, a\-z, 0\-9\) or the following special characters: \_\-\!"\#`\+\*\},\./ \. You can't change the name of a condition after you create it\.

1. Choose a **Region**\.

1. Choose a **Location type** and a country\. **Location type** is currently limited to **Country**\.

1. Choose **Add location**\.

1. Choose **Create**\.

## Editing Geo Match Conditions<a name="web-acl-geo-conditions-editing"></a>

You can add countries to or delete countries from your geo match condition\.<a name="web-acl-geo-conditions-editing-procedure"></a>

**To edit a geo match condition**

1. Sign in to the AWS Management Console and open the AWS WAF console at [https://console\.aws\.amazon\.com/waf/](https://console.aws.amazon.com/waf/)\. 

1. In the navigation pane, choose **Geo match**\.

1. In the **Geo match conditions** pane, choose the geo match condition that you want to edit\.

1. To add a country:

   1. In the right pane, choose **Add filter**\.

   1. Choose a **Location type** and a country\. **Location type** is currently limited to **Country**\.

   1. Choose **Add**\.

1. To delete a country:

   1. In the right pane, select the values that you want to delete\.

   1. Choose **Delete filter**\.

## Deleting Geo Match Conditions<a name="web-acl-geo-conditions-deleting"></a>

If you want to delete a geo match condition, you must first remove all countries in the condition and remove the condition from all the rules that are using it, as described in the following procedure\.<a name="web-acl-geo-conditions-deleting-procedure"></a>

**To delete a geo match condition**

1. Sign in to the AWS Management Console and open the AWS WAF console at [https://console\.aws\.amazon\.com/waf/](https://console.aws.amazon.com/waf/)\. 

1. Remove the geo match condition from the rules that are using it:

   1. In the navigation pane, choose **Rules**\.

   1. Choose the name of a rule that is using the geo match condition that you want to delete\.

   1. In the right pane, choose **Edit rule**\.

   1. Choose the **X** next to the condition you want to delete\.

   1. Choose **Update**\.

   1. Repeat for all the remaining rules that are using the geo match condition that you want to delete\.

1. Remove the filters from the condition you want to delete:

   1. In the navigation pane, choose **Geo match**\.

   1. Choose the name of the geo match condition that you want to delete\.

   1. In the right pane, choose the check box next to **Filter** in order to select all of the filters\.

   1. Choose the **Delete filter**\.

1. In the navigation pane, choose **Geo match**\.

1. In the **Geo match conditions** pane, choose the geo match condition that you want to delete\.

1. Choose **Delete** to delete the selected condition\.