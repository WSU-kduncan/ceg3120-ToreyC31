PART ONE


1. Create a VPC using the tag "YOURLASTNAME-VPC' with a /24 private IP address range  
Creates a Private cloud that someone can connect to an instance.
![Carroll-VPC](https://user-images.githubusercontent.com/77283021/153804860-2c0ed028-e99f-43cd-891f-d2a21154cfb2.PNG)

2. Create a subnet using the tag "YOURLASTNAME-Subnet" with an /28 private IP address range and attach it to your VPC
![Carroll-Subnet](https://user-images.githubusercontent.com/77283021/153804866-888c364a-5be1-4d23-9346-f27ea77407f2.PNG)

3. Create a gateway using the tag "YOURLASTNAME-gw" and attach it to your VPC
![Carroll-gw](https://user-images.githubusercontent.com/77283021/153804880-3fe36288-98ca-40d4-a797-a2d61ea4e997.PNG)

4. Create a route table and tag it with "YOURLASTNAME-routetable", attach it to your VPC, associate it with your subnet
Add a routing table rule that sends traffic to all destinations to your internet gateway
![Carroll-routetable](https://user-images.githubusercontent.com/77283021/153805309-6d1e36e7-7e6a-477c-97f5-c787cac495b0.PNG)


5. Create a security group, tag it with "YOURLASTNAME-sg".  
Allow SSH for a set of trusted networks including:  
Your home / where you usually connect to your instances from (I live on campus thus why it shows only 2)  
Wright State (addresses starting with 130.108)  
Instances within the VPC
![Carroll-sg](https://user-images.githubusercontent.com/77283021/153804876-db4e6aac-2dcb-4719-939b-5bb26c33c0bc.PNG)

PART TWO

1. Create an AMI:
- Ubuntu Server 18.04 LTS  
- t2.micro (Auto-Picked)
2. When I clicked "Configure Network Details" and went to the respected page, I scrolled down to "Network" and assigned it to my respected VPC.
3. I disabled this option, and plan on attaching an Elastic IP to the instance.
4. As suggested in class, I selected 16GB of gp2 SSD Volume Space.
5. When brought to the Tags page, there is not an automatic tag. This required me to click
"Add Tag". I changed the Key to be "Name" and Value to be "Carroll-instance" as requested per Project 2 guidelines
6. I want to Elastic IP's in AWS Environment. Clicked on "Allocate Elastic IP address".
7. Clicked "Add Tag" and gave the Key as "Name" with a value of "Carroll-EIP". Then clicked Allocate.
