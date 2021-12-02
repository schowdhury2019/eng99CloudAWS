# eng99CloudAWS

- create EC2 instance - VM 
- Ubuntu 18.04LTS
- Select the size of the VM
- Create Security Group
- SSH into machine with AWS key
- check VM - with update and upgrade
- install nginx to be accessible on public IP
- enable public ip
- get app folder using secure copy 'scp'
- install dependencies


Copy files into EC2 instance:

scp -i pem_file file_to_copy user@ip:/destination

example: scp -i "~/.ssh/eng99.pem" restaurant.py ubuntu@e***.com:/home/ubuntu/new_folder/restaurant.py

Regions and Availability Zones (AZ) 

Not every AZ has every services 

Configure security group:

Go in security tab and select security group
Add new inbound rule


![image](https://user-images.githubusercontent.com/14828358/144407299-7e2b7eb4-c4fe-4744-aa2b-f1fb2c84e7d3.png)

Steps to set up instance:

![image](https://user-images.githubusercontent.com/14828358/144407787-afcb3c44-4b77-4e00-8835-2c9755fddd0d.png)

Select free tier filter

![image](https://user-images.githubusercontent.com/14828358/144407926-42fd46f6-2fa6-42fe-b271-2b5b9afe0680.png)

![image](https://user-images.githubusercontent.com/14828358/144407995-6b230bb3-35be-4939-a62e-2330d44ea0c8.png)

Click Next

Step 3: Configure Instance

![image](https://user-images.githubusercontent.com/14828358/144436911-630261ce-ed00-4a7a-8004-ce483c0bb27d.png)

Step 4: Add Storage

Click Next

Step 5: Add Tags

![image](https://user-images.githubusercontent.com/14828358/144409066-a9e3d1e8-41a3-4fd7-adf8-7e2f5b6b90be.png)

![image](https://user-images.githubusercontent.com/14828358/144409178-0c50bacb-fd50-4ef4-9062-c68b41dff529.png)


![image](https://user-images.githubusercontent.com/14828358/144409355-b2e74ef9-666d-4a6f-b646-a1a19c9fca0c.png)



Specify new inbound rule to allow app to access database

![image](https://user-images.githubusercontent.com/14828358/144412565-c3bad5bd-bd61-4097-819a-990fe6a0c70b.png)



## Amazon Machine Image (AMI)

![image](https://user-images.githubusercontent.com/14828358/144434131-4c2dc9ce-01b4-497a-8493-16f7c04bf090.png)

Name it

Name = eng99_sunny_app_ami

## Monitoring

![image](https://user-images.githubusercontent.com/14828358/144445063-6979b7a2-b191-4d01-beae-fa0a7cf7a85f.png)

##CloudWatch - Monitoring Service

![image](https://user-images.githubusercontent.com/14828358/144445619-10eed2ea-b0ab-4a92-b7bd-42a516950f95.png)


