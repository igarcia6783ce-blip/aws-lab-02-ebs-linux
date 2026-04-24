# AWS Lab 02 — EC2 + EBS Linux Persistent Storage

## Overview
Hands-on AWS lab demonstrating creation and attachment of an EBS volume to an EC2 instance and configuring persistent Linux storage using `/etc/fstab`.

## Objectives
- Launch EC2 instance
- Create and attach EBS volume
- Format Linux filesystem
- Mount volume to directory
- Configure persistent mount using `/etc/fstab`
- Verify storage after reboot

## Environment
- AWS EC2 (Amazon Linux)
- Amazon EBS
- Linux CLI
- SSH

- ## Steps Performed
1. Launched EC2 instance (Amazon Linux)
2. Created new EBS volume in same Availability Zone
3. Attached EBS volume to EC2 instance
4. Formatted volume using mkfs (ext4)
5. Created mount directory (/data)
6. Mounted volume to /data
7. Retrieved UUID using blkid
8. Updated /etc/fstab for persistent mounting
9. Rebooted instance to verify persistence

10. ## Commands Used
lsblk
sudo mkfs -t ext4 /dev/xvdf
sudo mkdir /data
sudo mount /dev/xvdf /data
sudo blkid
sudo nano /etc/fstab
sudo mount -a


## Skills Demonstrated
- AWS EBS provisioning
- Amazon EBS storage
- Linux administration
- Filesystem mounting
- Persistent storage configuration

## Outcome
Successfully configured persistent storage on an EC2 instance using an EBS volume and /etc/fstab, ensuring the volume automatically mounts after reboot.
