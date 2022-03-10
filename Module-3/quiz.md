# Questions with correct answers and explanations

## Which statement best describes an Availability Zone?

a) A geographical area that contains AWS resources

b) A single data center or group of data centers within a Region --correct

c) A data center that an AWS service uses to perform service-specific operations

d) A service that you can use to run AWS infrastructure within your own on-premises data center in a hybrid approach

### Explanation for other options

    A Region is a geographical area that contains AWS resources.

    An edge location is a data center that an AWS service uses to perform service-specific operations. Edge locations are examined in the next section of this module.

    AWS Outposts is a service that you can use to run AWS infrastructure, services, and tools in your own on-premises data center in a hybrid approach. AWS Outposts is explored later in this module.

Learn more:

[AWS global infrastructure](https://aws.amazon.com/about-aws/global-infrastructure)
[Regions and Availability Zones](https://aws.amazon.com/about-aws/global-infrastructure/regions_az)

------------

## Which statement is TRUE for the AWS global infrastructure?

a) A Region consists of a single Availability Zone.

b) An Availability Zone consists of two or more Regions.

c) A Region consists of two or more Availability Zones. -- correct

d) An Availability Zone consists of a single Region.

### Explanation for other options

    The correct response option is A Region consists of two or more Availability Zones.

    For example, the South America (São Paulo) Region is sa-east-1. It includes three Availability Zones: sa-east-1a, sa-east-1b, and sa-east-1c.

Learn more:

[AWS global infrastructure](https://aws.amazon.com/about-aws/global-infrastructure)
[Regions and Availability Zones](https://aws.amazon.com/about-aws/global-infrastructure/regions_az)

------------

## Which factors should be considered when selecting a Region? (Select TWO.)

a) Compliance with data governance and legal requirements -- correct

b) Proximity to your customers --correct

c) Access to 24/7 technical support

d) Ability to assign custom permissions to different users

e) Access to the AWS Command Line Interface (AWS CLI)

### Explanation for other options

    The correct two response options are:

    - Compliance with data governance and legal requirements
    - Proximity to your customers
    
    Two other factors to consider when selecting a Region are pricing and the services that are available in a Region.

    The other response options are incorrect because:

    - The level of support that you choose is not determined by Region. AWS Support plans are explored later in this course.
    - Assigning custom permissions to different users is a feature that is possible in all AWS Regions.
    The AWS Command Line Interface (AWS CLI) is available in all AWS Regions.

------------

## Which statement best describes Amazon CloudFront?

a) A service that enables you to run infrastructure in a hybrid cloud approach

b) A serverless compute engine for containers

c) A service that enables you to send and receive messages between software components through a queue

d) A global content delivery service --correct

### Explanation for other options

    Amazon CloudFront is a content delivery service. It uses a network of edge locations to cache content and deliver content to customers all over the world. When content is cached, it is stored locally as a copy. This content might be video files, photos, webpages, and so on.

    The other response options are incorrect because:

    - AWS Outposts is a service that enables you to run infrastructure in a hybrid cloud approach.
    - AWS Fargate is a serverless compute engine for containers.
    - Amazon Simple Queue Service (Amazon SQS) is a service that enables you to send, store, and receive messages between software components through a queue.


------------

## Which site does Amazon CloudFront use to cache copies of content for faster delivery to users at any location?

a) Region

b) Availability Zone

c) Edge location --correct

d) Origin

### Explanation for other options

    A Region is a separate geographical location with multiple locations that are isolated from each other.

    An Availability Zone is a fully isolated portion of the AWS global infrastructure.

    An origin is the server from which CloudFront gets your files. Examples of CloudFront origins include Amazon Simple Storage Service (Amazon S3) buckets and web servers. Note: Amazon S3 is explored later in this course.


## Which action can you perform with AWS Outposts?

a) Automate actions for AWS services and applications through scripts.

b) Access wizards and automated workflows to perform tasks in AWS services.

c) Develop AWS applications in supported programming languages.

d) Extend AWS infrastructure and services to your on-premises data center. --correct

### Explanantion for other options

    The AWS Command Line Interface (AWS CLI) is used to automate actions for AWS services and applications through scripts.

    The AWS Management Console includes wizards and workflows that you can use to complete tasks in AWS services.

    Software development kits (SDKs) enable you to develop AWS applications in supported programming languages.
