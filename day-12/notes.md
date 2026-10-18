\# Day 12 - AWS EBS (Elastic Block Store)



\## 1. What is Amazon EBS?



EBS stands for Elastic Block Store.



Amazon EBS is a block storage service provided by AWS. It provides storage volumes that can be attached to EC2 instances.



We use EBS to store operating system files, application files, and other data.



\## 2. What is a Storage Volume?



A storage volume is like a virtual hard disk.



Just as a computer needs a hard disk to store files, an EC2 instance can use an EBS volume to store data.



\## 3. Relationship Between EC2 and EBS



\- EC2 provides virtual computing capacity.

\- EBS provides block storage.

\- An EBS volume can be attached to an EC2 instance.

\- The operating system can use the attached volume to store files and data.



Example:



An EC2 instance runs a web application, while an EBS volume stores application files and other data.



\## 4. Important EBS Features



\### Persistent Storage



EBS volumes are designed to retain data independently of the running life of an EC2 instance.



Stopping an EC2 instance does not normally delete its attached EBS volumes.



\### Volume Attachment



An EBS volume can be attached to an EC2 instance, subject to AWS compatibility and attachment limits.



\### Snapshots



An EBS snapshot is a point-in-time backup of an EBS volume.



Snapshots can help recover data or create new volumes.



\### Resizing



EBS volumes can generally be increased in size. The operating system's partition or file system may also need to be extended.



\## 5. EBS vs Instance Store



\### EBS



\- Persistent block storage.

\- Data is designed to remain after an instance stops.

\- Can be backed up using snapshots.



\### Instance Store



\- Temporary storage physically associated with the host computer.

\- Data may be lost when an instance is stopped, terminated, or otherwise loses its underlying host, depending on the event and instance type.

\- Useful for temporary data and caches.



\## 6. EBS Volume Types



Common EBS volume types include:



\- General Purpose SSD (gp3): General-purpose workloads.

\- General Purpose SSD (gp2): Earlier general-purpose SSD option.

\- Provisioned IOPS SSD (io2): Workloads needing high, consistent I/O performance.

\- Throughput Optimized HDD (st1): Throughput-intensive workloads.

\- Cold HDD (sc1): Infrequently accessed, throughput-oriented workloads.



HDD volume types are not suitable as boot volumes.



\## 7. What Happens When an EC2 Instance Stops?



Stopping an EC2 instance normally preserves its attached EBS volumes and their data.



Compute charges stop while the instance is stopped, but storage charges for retained EBS volumes generally continue.



\## 8. What Happens When an EC2 Instance Is Terminated?



When an EC2 instance is terminated, an attached EBS volume configured for deletion on termination may be deleted.



A volume configured to be retained can remain in the AWS account.



Always check the volume's settings before terminating an instance.



\## 9. What Is an EBS Snapshot?



A snapshot is a point-in-time backup of an EBS volume.



Snapshots are useful for:



\- Data protection.

\- Disaster recovery.

\- Creating new EBS volumes.

\- Preserving data before making major changes.



Snapshots are stored and billed separately according to AWS pricing rules.



\## 10. Day 12 Practical Learning



1\. Open the AWS Management Console.

2\. Navigate to EC2.

3\. Open the Volumes section under Elastic Block Store.

4\. Identify the volume attached to your practice EC2 instance.

5\. Observe its size, state, volume type, and Availability Zone.

6\. Do not delete or detach a volume that contains important data.



Optional practice: Create a small test EBS volume in the same Availability Zone as your EC2 instance. Check the current AWS charges and free-tier eligibility before creating resources.



\## 11. What I Learned



Today I learned that EBS is block storage for EC2 instances. I learned about EBS volume types, persistent storage, snapshots, instance store, and what happens to EBS volumes when an EC2 instance stops or terminates.



\## 12. Key Takeaway



EC2 provides computing capacity, while EBS provides persistent block storage. Understanding how they work together is important for managing AWS infrastructure.

