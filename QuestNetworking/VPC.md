## Amazon Virtual Private Cloud, VPC Overview. 
Amazon Virtual Private Cloud. 
    Amazon VPC is like your own private cloud within the AWS Cloud. It lets you provision a logically isolated section of the AWS Cloud where you can launch AWS resources in virtual network that you define. This is a virtual network dedicated to your AWS account. Alternatively, your AWS account comes with a pre-configured default VPC in each region. 
    
    You can launch your resources into the default VPC right away. Amazon VPC also provides you with complete control over your virtual networking environment, including selection of your own IP address range, creation of subnets, and configuration of route tables and network gateways. 
    
    To get started with creating a VPC, you must assign it with a range of private IP addresses. Amazon VPC supports IPv4 and IPv6. Your resources can communicate over IPv4 or IPv6 or both. By default, it uses the IPv4 addressing protocol. 
    
    You can also bring your own IP prefixes. A VPC spans all of the availability zones in the region. After creating a VPC, you can add one or more subnets in each availability zone. A subnet is a partition of a VPC's IP address range. For example, your VPC has a total of 1024 IP addresses, and you configure four subnets, each has 251 IP addresses. Each subnet must reside entirely within one availability zone. You can launch instances into subnets in multiple availability zones to improve fault tolerance and hence building highly available applications. 
    
    Creating multiple VPCs is supported. In one AWS account, you can create up to five VPCs per region by default. If more is required, this limit can be increased through AWS support. 
    
    Now, let's talk about the key benefits of Amazon VPC. First, it is simple. 
    
    Using the AWS Management Console, VPC can be quickly and easily created. You spend less time setting up and managing, so you can concentrate on building the applications that run in your VPCs. Customizable. You can easily customize the network configuration of your Amazon VPC. For example, you can create a public facing subnet for your web servers that have access to the internet. You can also place your backend systems, such as databases or application servers in a private facing subnet with no internet access. When you configure VPC to connect to your corporate network, it can serve as an extension of your own data center. 
    
    In addition, VPC can also be connected to other VPCs. Secure Amazon VPC provides multiple layer of advanced security features, such as network access control lists, NACLs and security groups to enable inbound and outbound filtering at the subnet and instance level. In addition, you can store data in Amazon S3 and restrict access so that it's only accessible from instances inside your VPC. 