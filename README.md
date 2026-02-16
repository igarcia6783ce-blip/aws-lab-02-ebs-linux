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

## Steps Performed
1. Launched EC2 instance
2. Created EBS volume
3. Attached volume to EC2
4. Formatted filesystem (`mkfs`)
5. Created mount directory
6. Mounted volume
7. Updated `/etc/fstab`
8. Reboot verification

## Skills Demonstrated
- AWS EC2 provisioning  
- Amazon EBS storage  
- Linux administration  
- Filesystem mounting  
- Persistent storage configuration
