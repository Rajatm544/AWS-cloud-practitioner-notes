# Questions with correct answers and explanations

## Which statement best describes an AWS account’s default network access control list?

a) It is stateless and denies all inbound and outbound traffic.

b) It is stateful and allows all inbound and outbound traffic.

c) It is stateless and allows all inbound and outbound traffic. --correct

d) It is stateful and denies all inbound and outbound traffic.

### Explanation for other options

    Network access control lists (ACLs) perform stateless packet filtering. They remember nothing and check packets that cross the subnet border each way: inbound and outbound.

    Each AWS account includes a default network ACL. When configuring your VPC, you can use your account’s default network ACL or create custom network ACLs.

    By default, your account’s default network ACL allows all inbound and outbound traffic, but you can modify it by adding your own rules. For custom network ACLs, all inbound and outbound traffic is denied until you add rules to specify which traffic should be allowed. Additionally, all network ACLs have an explicit deny rule. This rule ensures that if a packet doesn’t match any of the other rules on the list, the packet is denied.

## Which statement best describes DNS resolution?

a) Launching resources in a virtual network that you define

b) Storing local copies of content at edge locations around the world

c) Connecting a VPC to the internet

d) Translating a domain name to an IP address --correct

### Explanation for other options

    The correct response option is Translating a domain name to an IP address.

    For example, if you want to visit AnyCompany’s website, you enter the domain name into your PC and this request is sent to a DNS server. Next, the DNS server asks the web server for the IP address that corresponds to AnyCompany’s website. The web server responds by providing the IP address for AnyCompany’s website, 192.0.2.0.

## Your company has an application that uses Amazon EC2 instances to run the customer-facing website and Amazon RDS database instances to store customers’ personal information. How should the developer configure the VPC according to best practices?

a) Place the Amazon EC2 instances in a private subnet and the Amazon RDS database instances in a public subnet.

b) Place the Amazon EC2 instances in a public subnet and the Amazon RDS database instances in a private subnet. --correct

c) Place the Amazon EC2 instances and the Amazon RDS database instances in a public subnet.

d) Place the Amazon EC2 instances and the Amazon RDS database instances in a private subnet.

### Explanation for other options

    The correct response option is Place the Amazon EC2 instances in a public subnet and the Amazon RDS databases instances in a private subnet.

    A subnet is a section of a VPC in which you can group resources based on security or operational needs. Subnets can be public or private.

    Public subnets contain resources that need to be accessible by the public, such as an online store’s website.

    Private subnets contain resources that should be accessible only through your private network, such as a database that contains customers’ personal information and order histories.

## Which component or service can be used to establish a private dedicated connection between your company’s data center and AWS?

a) Private subnet

b) DNS

c) AWS Direct Connect --correct

d) Amazon CloudFront

### Explanation for other options

    The correct response option is AWS Direct Connect.

    The other response options are incorrect because:

    A private subnet is a section of a VPC in which you can group resources that should be accessed only through your private network. Although it is private, it is not used for establishing a connection between a data center and AWS.
    DNS stands for Domain Name System, which is a directory used for matching domain names to IP addresses.
    Amazon CloudFront is a content delivery service. You can use CloudFront to store cached copies of your content at edge locations that are close to your customers.

## Which statement best describes security groups?

a) They are stateful and deny all inbound traffic by default. --correct

b) They are stateful and allow all inbound traffic by default.

c) They are stateless and deny all inbound traffic by default.

d) They are stateless and allow all inbound traffic by default.

### Explanation for other options

    The correct response option is Security groups are stateful and deny all inbound traffic by default.

    Security groups are stateful. This means that they use previous traffic patterns and flows when evaluating new requests for an instance.

    By default, security groups deny all inbound traffic, but you can add custom rules to fit your operational and security needs.

## Which component is used to connect a VPC to the internet?

a) Public subnet

b) Edge location

c) Security group

d) Internet gateway --correct

### Explanation for other options

    The correct response option is Internet gateway.

    The other response options are incorrect because:

    A public subnet is a section of a VPC that contains public-facing resources.
    An edge location is a site that Amazon CloudFront uses to store cached copies of your content for faster delivery to customers.
    A security group is a virtual firewall that controls inbound and outbound traffic for an Amazon EC2 instance

## Which service is used to manage the DNS records for domain names?

a) Amazon Virtual Private Cloud

b) AWS Direct Connect

c) Amazon CloudFront

d) Amazon Route 53 --correct

### Explanation for other options

    Amazon Route 53 is a DNS web service. It gives developers and businesses a reliable way to route end users to internet applications that host in AWS.

    Another feature of Route 53 is the ability to manage the DNS records for domain names. You can transfer DNS records for existing domain names managed by other domain registrars. You can also register new domain names directly in Route 53.

    The other response options are incorrect because:

    Amazon Virtual Private Cloud (Amazon VPC) is a service that enables you to provision an isolated section of the AWS Cloud. In this isolated section, you can launch resources in a virtual network that you define.

    AWS Direct Connect is a service that enables you to establish a dedicated private connection between your data center and VPC.  

    Amazon CloudFront is a content delivery service. It uses a network of edge locations to cache content and deliver content to customers all over the world.
