# Availability Zones

![AZ](https://user-images.githubusercontent.com/42696800/154280062-f4df29cb-47c9-4c50-a343-b5b7497477bc.png)

An **Availability Zone** is a single data center or a group of data centers within a Region. Availability Zones are located tens of miles apart from each other. This is close enough to have low latency (the time between when content requested and received) between Availability Zones. However, if a disaster occurs in one part of the Region, they are distant enough to reduce the chance that multiple Availability Zones are affected.

## Running Amazon EC2 instances in multiple Availability Zones

### STEP 1: Amazon EC2 instance in a single Availability Zone

![step1](https://user-images.githubusercontent.com/42696800/154280328-60cfff02-6153-40c0-9a52-bad628483980.png)

Suppose that you’re running an application on a single Amazon EC2 instance in the Northern California Region. The instance is running in the us-west-1a Availability Zone. If us-west-1a were to fail, you would lose your instance.

### Step 2: Amazon EC2 instances in multiple Availability Zones

![step2](https://user-images.githubusercontent.com/42696800/154280536-fccded9b-3c60-4d3e-98cf-6e2c349009ae.png)

A best practice is to run applications across at least two Availability Zones in a Region. In this example, you might choose to run a second Amazon EC2 instance in us-west-1b.

### Step 3: Availability Zone failure

![step 3](https://user-images.githubusercontent.com/42696800/154281057-8042cbc2-9543-4f78-bcf8-03dd453a7ded.png)

If us-west-1a were to fail, your application would still be running in us-west-1b.
