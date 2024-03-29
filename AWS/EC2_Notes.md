# EC2 Notes

Amazon Elastic Compute Cloud (EC2) is a way to run virtual servers in cloud.

EC2 Host server or EC2 Hosts ( Physical hardware of the EC2 service) is maintained and managed by Amazon AWS.

EC2 Instance is a virtual server managed by users, which runs on top of EC2 Hosts.

## EC2 Instance Type

EC2 Instance type (Hardware profile) is a combination of CPU, Memory, Storage and Networking.

Each instance type is targeted for certain types of work load.

| Category | Families | Purpose/Design |
| ----------- | ----------- | ----------- |
| General Purpose | Mac, T4g, T3, T3a, T2, M6g, M6i, M5, M5a, M5n, M5zn, M5, A1 | General Purpose Instances provide a balance on compute, memory, and networking resources, and can be used for a variety of diverse workloads. |
| Compute Optimized | C6g, C6gn, C6i, C5, C5a, C5n, C4 | Compute optimized are ideal for compute bound applications that benefit from high performance processors. |
| Memory Optimized | R6g, R5, R5a, R5b, R5n, R4, X2gd, X1e, X1, High Memory, z1d | Memory optimized instances are designed to deliver fast performance for workloads that process large data sets in memory. |
| Accelerated Computing | P4, P3, P2, DL1, Inf1, G5, G4dn, G4ad, G3, F1, VT1 | Accelerated Computing instances use hardware accelerators, or co-processors to perform functions such as floating-point number calculations, graphics processing, or data pattern matching. |
| Storage Optimized | I3, I3en, D2, D4, D3en, H1 | This instance family provides Non-Volatile Memory Express (NVMe) SSD-Backed instance storage optimized for low latency, very high random I/O performance, high sequential read throughput and high IOPS at a low cost. |

EC2 instance can run different OS (windows, linux, macos).

Amazon Machine Image (AMI) defines the configuration (instance type + OS + user config) of the instance.

EBS snapshot is a point in time backup of an instance. AMI can be created from EBS snapshot and is called customised AMI.

## EC2 Service

EC2 is a regional service. 

![EC2 service](./assets/images/AWS_EC2.png)

EBS Volume is hard drive attached to instance.

Security group controls the inbound and outbound traffic to the instance.

## EC2 Instance Launch and Connection



