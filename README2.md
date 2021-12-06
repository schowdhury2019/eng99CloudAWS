# Week 4 VPC and CICD


![image](https://user-images.githubusercontent.com/14828358/144827863-ddaba37f-9d3e-4eb1-b0e4-bdfd8f9afb0f.png)





![image](https://user-images.githubusercontent.com/14828358/144831914-f1084794-2c5e-48b0-9234-91d4669ea713.png)




## Network Access Control Layer (NACL)

  * An optional layer of security for your VPC that acts as a firewall for controlling traffic in and out of one or more subnets 

## Route Tables

  * A route table contains a set of rules, called routes, that are used to determine where network traffic from your subnet or gateway is directed.






## Step 1: Create VPC


## Step 2: Internet Gateway

### Attach IG to VPC

## Step 3: Public Subnet for our App

## Step 4: Create Routing Table with Routes and Rules

### Edit Routes to allow IG and VPC

### Associate our RT to our public subnet


- Create security group now or when app is launched
- port 22 from my_ip
- port 3000
- port 80 HTTP with cert for security
- HTTP - SSL cert
