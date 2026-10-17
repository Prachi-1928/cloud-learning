# Day 11 - EC2 Linux and SSH Practice

## What is SSH?

SSH stands for Secure Shell.

SSH is a protocol used to securely connect to and manage a remote computer over a network.

In cloud computing, SSH is commonly used to connect to Linux EC2 instances.

## SSH Connection

The basic SSH connection looks like:

```bash
ssh -i "private-key.pem" username@public-ip
```

The command contains:

- `ssh` - Secure Shell command
- `-i` - Specifies the private key
- `username` - Linux user
- `public-ip` - Public IP address of the EC2 instance

## Why is SSH Important?

SSH allows a cloud engineer to remotely manage a Linux server.

For example, after connecting to an EC2 instance, we can:

- Run Linux commands
- Install software
- Create files
- Configure applications
- Check system information
- Manage services

## Basic Linux Commands on EC2

### whoami

Shows the current Linux user.

```bash
whoami
```
