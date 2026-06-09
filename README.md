 aws-ebs-volume-management
# AWS EBS Volume Management

## Project Overview
This project demonstrates attaching, formatting, mounting, and resizing Amazon EBS volumes on an EC2 instance.

## Services Used
- Amazon EC2
- Amazon EBS
- Linux

## Steps Performed
1. Created an EBS volume.
2. Attached the volume to an EC2 instance.
3. Verified the device using lsblk.
4. Formatted the volume.
5. Mounted the volume.
6. Configured automatic mounting using /etc/fstab.
7. Extended the volume size.
8. Resized the filesystem.

## Commands Used

bash
lsblk
sudo mkfs -t xfs /dev/nvme1n1
sudo mkdir /data
sudo mount /dev/nvme1n1 /data
df -h
sudo blkid
sudo nano /etc/fstab
sudo growpart
sudo xfs_growfs
