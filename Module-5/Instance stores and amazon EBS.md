# Instance stores

Block-level storage volumes behave like physical hard drives.

An [instance store](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/InstanceStorage.html) provides temporary block-level storage for an Amazon EC2 instance. An instance store is disk storage that is physically attached to the host computer for an EC2 instance, and therefore has the same lifespan as the instance. When the instance is terminated, you lose any data in the instance store.

## Step 1

![image](https://user-images.githubusercontent.com/42696800/158979232-194f274c-5d47-4460-ae94-2ffddaf98a0d.png)

## Step 2

![image](https://user-images.githubusercontent.com/42696800/158979324-ab335135-fdc1-4c28-b610-f9b5b65f3da9.png)

## Step 3

![image](https://user-images.githubusercontent.com/42696800/158979424-60ccf448-e2b6-4f54-857b-2ce06dfad02c.png)


# Amazon Elastic Block Store (EBS)

![image](https://user-images.githubusercontent.com/42696800/158979586-305cb939-7c2c-42f5-bb35-7894f9452a3a.png)

[Amazon Elastic Block Store (Amazon EBS)](https://aws.amazon.com/ebs) is a service that provides block-level storage volumes that you can use with Amazon EC2 instances. If you stop or terminate an Amazon EC2 instance, all the data on the attached EBS volume remains available.

To create an EBS volume, you define the configuration (such as volume size and type) and provision it. After you create an EBS volume, it can attach to an Amazon EC2 instance.

Because EBS volumes are for data that needs to persist, it’s important to back up the data. You can take incremental backups of EBS volumes by creating Amazon EBS snapshots.

# Amazon EBS snapshots

![image](https://user-images.githubusercontent.com/42696800/158979773-9501f777-9b37-484a-a8d7-7c9bc7b8752b.png)

An [EBS snapshot](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/EBSSnapshots.html) is an incremental backup. This means that the first backup taken of a volume copies all the data. For subsequent backups, only the blocks of data that have changed since the most recent snapshot are saved.

Incremental backups are different from full backups, in which all the data in a storage volume copies each time a backup occurs. The full backup includes data that has not changed since the most recent backup.
