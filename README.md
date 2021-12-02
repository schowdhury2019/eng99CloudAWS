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



Configure security group:

Go in security tab and select security group
Add new inbound rule


![image](https://user-images.githubusercontent.com/14828358/144407299-7e2b7eb4-c4fe-4744-aa2b-f1fb2c84e7d3.png)

