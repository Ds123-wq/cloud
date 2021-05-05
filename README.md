# 🔰 Terraform Automation 🔰

### Task Description 

🔅   Write an Infrastructure as code using terraform, which automatically create a VPC.
🔅   In that VPC we have to create 2 subnets:
     1.   public  subnet [ Accessible for Public World! ] 
     2.   private subnet [ Restricted for Public World! ]
🔅 Create a public facing internet gateway for connect our VPC/Network to the internet world and attach this gateway to our VPC.
🔅 Create  a routing table for Internet gateway so that instance can connect to outside world, update and associate it with public subnet.
🔅  Create a NAT gateway for connect our VPC/Network to the internet world  and attach this gateway to our VPC in the public network
🔅  Update the routing table of the private subnet, so that to access the internet it uses the nat gateway created in the public subnet
🔅  Launch an ec2 instance which has Wordpress setup already having the security group allowing  port 80 sothat our client can connect to our wordpress site. Also attach the key to instance for further login into it.
🔅  Launch an ec2 instance which has MYSQL setup already with security group allowing  port 3306 in private subnet so that our wordpress vm can connect with the same. Also attach the key with the same.

#### Note: Wordpress instance has to be part of public subnet so that our client can connect our site. mysql instance has to be part of private  subnet so that outside world can't connect to it.Also add auto ip assign and auto dns name assignment option to be enabled.

For more detailed visit https://www.linkedin.com/feed/update/urn:li:activity:6716711135258652673
