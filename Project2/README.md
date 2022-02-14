1. Create a VPC using the tag "YOURLASTNAME-VPC' with a /24 private IP address range
![Carroll-VPC](https://user-images.githubusercontent.com/77283021/153796469-c6c14032-41bb-4d56-a807-1081395c0bcc.PNG)

2. Create a subnet using the tag "YOURLASTNAME-Subnet" with an /28 private IP address range and attach it to your VPC
![Carroll-Subnet](https://user-images.githubusercontent.com/77283021/153796900-e4c07684-1752-460d-a251-0ac3992e536f.PNG)

3. Create a gateway using the tag "YOURLASTNAME-gw" and attach it to your VPC
![carroll-gw](https://user-images.githubusercontent.com/77283021/153802462-46ffc5d4-ebff-4095-b638-7cb43ec89dc5.PNG)

4. Create a route table and tag it with "YOURLASTNAME-routetable", attach it to your VPC, associate it with your subnet
Add a routing table rule that sends traffic to all destinations to your internet gateway

5. Create a security group, tag it with "YOURLASTNAME-sg". Allow SSH for a set of trusted networks including:
- Your home / where you usually connect to your instances from
- Wright State (addresses starting with 130.108)
- Instances within the VPC
- Then attach it to your VPC
Image should include your Inbound rules
