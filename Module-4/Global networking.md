# Domain Name System (DNS)

Suppose that AnyCompany has a website hosted in the AWS Cloud. Customers enter the web address into their browser, and they are able to access the website. This happens because of **Domain Name System (DNS)** resolution. DNS resolution involves a customer DNS resolver communicating with a company DNS server.

You can think of DNS as being the phone book of the internet. DNS resolution is the process of translating a domain name to an IP address.

![image](https://user-images.githubusercontent.com/42696800/158956417-ebbd92a2-e1e6-4741-8d93-ce1537116d57.png)

For example, suppose that you want to visit AnyCompany’s website.

1) When you enter the domain name into your browser, this request is sent to a customer DNS resolver.

2) The customer DNS resolver asks the company DNS server for the IP address that corresponds to AnyCompany’s website.

3) The company DNS server responds by providing the IP address for AnyCompany’s website, 192.0.2.0.

## Amazon Route 53

[Amazon Route 53](https://aws.amazon.com/route53) is a DNS web service. It gives developers and businesses a reliable way to route end users to internet applications hosted in AWS.

Amazon Route 53 connects user requests to infrastructure running in AWS (such as Amazon EC2 instances and load balancers). It can route users to infrastructure outside of AWS.

Another feature of Route 53 is the ability to manage the DNS records for domain names. You can register new domain names directly in Route 53. You can also transfer DNS records for existing domain names managed by other domain registrars. This enables you to manage all of your domain names within a single location.

In the previous module, you learned about Amazon CloudFront, a content delivery service. The following example describes how Route 53 and Amazon CloudFront work together to deliver content to customers.

### Example: How Amazon Route 53 and Amazon CloudFront deliver content

![image](https://user-images.githubusercontent.com/42696800/158956629-e007e3a2-3f2e-49bf-9fd7-11791c73dabb.png)

Suppose that AnyCompany’s application is running on several Amazon EC2 instances. These instances are in an Auto Scaling group that attaches to an Application Load Balancer.

1) A customer requests data from the application by going to AnyCompany’s website.

2) Amazon Route 53 uses DNS resolution to identify AnyCompany.com’s corresponding IP address, 192.0.2.0. This information is sent back to the customer.

3) The customer’s request is sent to the nearest edge location through Amazon CloudFront.

4) Amazon CloudFront connects to the Application Load Balancer, which sends the incoming packet to an Amazon EC2 instance.