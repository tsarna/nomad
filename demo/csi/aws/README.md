# AWS CSI Plugins

Configurations are provided here for [Elastic Block Store](https://aws.amazon.com/ebs/) and [Elastic Filesystem](https://aws.amazon.com/efs/) CSI drivers for use on Amazon Web Services.

## Elastic Block Store

EBS provides virtual block disks. Disks are tied to an availability zone, and aside from [io1 multi-attach](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/ebs-volumes-multi.html), which requires special filesystems to use in read-write mode, may only be used by a single node at a time.

## Elastic File Store

EFS provides a shared network filesystem over NFSv4. An EFS filesystem may be used within an AWS region, not just an availability zone, and can be accessed even in read-write mode by multiple nodes at once.
