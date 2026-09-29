# Day 10 - AWS EC2: Launching Your First Instance



## What is EC2?



EC2 stands for Elastic Compute Cloud.



Amazon EC2 is an AWS service that provides virtual servers in the cloud.



Instead of buying and maintaining a physical server, we can create a virtual server using EC2.



---



## What is an EC2 Instance?



An EC2 instance is a virtual machine running in AWS.



We can use an EC2 instance to:



- Run applications

- Host websites

- Run backend servers

- Store and process data

- Perform computing tasks



---



## Why is EC2 called Elastic?



Elastic means resources can be increased or decreased according to requirements.



For example:



If an application needs more computing power, we can choose a more powerful instance.



If we need fewer resources, we can use a smaller instance.



---



## Important EC2 Concepts



### 1. AMI



AMI stands for Amazon Machine Image.



An AMI is a template used to create an EC2 instance.



It contains the operating system and other required software.



Example:



Ubuntu can be selected as an operating system for an EC2 instance.



---



### 2. Instance Type



Instance type determines the computing resources available to the instance.



It determines things such as:



- CPU

- Memory

- Network performance



Different instance types are designed for different workloads.



---



### 3. Key Pair



A key pair is used to securely connect to an EC2 instance.



It contains:



- Public key

- Private key



The private key must be kept secure.



Never share the private key with anyone.



---



### 4. Security Group



A security group acts like a virtual firewall for an EC2 instance.



It controls which network traffic is allowed to reach the instance.



For example:



SSH uses port 22.



HTTP uses port 80.



HTTPS uses port 443.



---



### 5. Public IP Address



An EC2 instance can have a public IP address.



A public IP allows the instance to communicate over the internet.



---



### 6. Private IP Address



A private IP address is used for communication inside the AWS network.



It is not directly accessible from the public internet.



---



## Launching an EC2 Instance



Basic steps:



1. Open the AWS Management Console.

2. Open the EC2 service.

3. Choose the required AWS Region.

4. Click Launch Instance.

5. Give the instance a name.

6. Select an AMI.

7. Select an instance type.

8. Create or select a key pair.

9. Configure the security group.

10. Launch the instance.



---



## Connecting to an EC2 Instance



After launching the instance:



1. Open the EC2 console.

2. Select the running instance.

3. Click Connect.

4. Choose the appropriate connection method.

5. Follow the connection instructions.



For a Linux EC2 instance, SSH is commonly used.



---



## What is SSH?



SSH stands for Secure Shell.



SSH allows us to securely connect to a remote computer over a network.



Example:



A developer can use SSH to connect from their local computer to a Linux EC2 instance.



---



## SSH Port



SSH normally uses port 22.



The EC2 security group must allow SSH traffic for the connection to work.



---



## EC2 Lifecycle



An EC2 instance can have different states.



Common states include:



- Pending

- Running

- Stopping

- Stopped

- Terminated



---



## Stop vs Terminate



### Stop



Stopping an instance shuts down the instance but keeps it available to start again later.



### Terminate



Terminating an instance permanently removes the instance.



Therefore, terminate should be used carefully.



---



## Day 10 Hands-On Task



I launched an EC2 instance using the AWS Management Console.



I selected:



- An AMI

- An instance type

- A key pair

- A security group



I started the EC2 instance and observed its public IP address.



I connected to the Linux EC2 instance using SSH.



---



## What I Learned



Today I learned:



- What EC2 is

- What an EC2 instance is

- What an AMI is

- What an instance type is

- What a key pair is
- What a security group is

- What a public IP is

- What a private IP is

- What SSH is

- Why SSH uses port 22

- Difference between stopping and terminating an EC2 instance



---



## Important Security Rule



Never share my EC2 private key.



Never upload the private key to GitHub.



Never put passwords, secret keys, or credentials inside GitHub notes.

