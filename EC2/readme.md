# `Compute Services`

## `EC2 Elastic compute cloud`

### `Compute Capacity` : 

The ability of AWS to launch N number of servers within few min is called as Compute Capacity of AWS

![amazonEC2](/images/readme/amazonec2Intro.png)

AMI + IT + EBS = Rq config == EC2 Instance 
## `How to launch a windows EC2 Instance `

- Go to AWS Management console

- Select the server Asia Pacific (Mumbai) 

- - We are choosing Mumbai because it is nearest and the latency will be the lowest

- Go to the search bar and type `ec2` 

![searchMark](/images/readme/searchMark.jpeg)
- There check the availability zones of mumbai names as 
- - ap-south-1a
- - ap-south-1b
- - ap-south-1c
- - But the region is ap-south-1

## There are two ways to launch the EC2 instance
- By clicking Instance (running ) from the resouce panel 
- - This gives the running instances immediately
- By directly clicking the Instance button in the Same page

![launchInstanceRunning](/images/readme/launchinstancerunning.jpeg)

### Procedure
-  Click on the `Launch instance` button 

![launchinstance](/images/readme/launchInstancerunning2.jpeg)
-  Then there It will be aksing you the `name and tags `
- -  The tags are used to define the which types of instance it is

![windows1](/images/readme/windows1.jpeg)
-  Choose the `Application and Os Images (Amazon Machine Image)` 
- -  OS Images then find the windows image then check for the free tier image 

![windows2](/images/readme/windows2.jpeg)

![windows3](/images/readme/windows3.jpeg)

![windows4](/images/readme/windows4.jpeg)
-  Then Choose the `Instance Type`
- - CPU + Ram (Check the t2.micro - `this is free tier eligible`)

![windows5](/images/readme/windows5.jpeg)

- `Key Pair (login)`

![windows6](/images/readme/windows6.jpeg)

![windows7](/images/readme/windows7.jpeg)

- `In Security Group name` change it to your desired name to `win` so that you can identify it  
- - Also put a `Description` there
- - Then the Inbound Security Group Rules are automaticlly be defined by AWS
- - `Win = RDP : 3389` this port is used only by windows
- - `Source` will be set to anywhere you can change it 

- - It requires a key to enter ther which will be in the format of `.pem` it stands for `privacy enhanced many` that is done in t`he Keypair`

![windows9](/images/readme/windows9.jpeg)
![windows10](/images/readme/windows10.jpeg)

- `Configuration Storage`

- - EBS -> Elastic Block store
- - in AWS is root is windows C drive
- - 30gb is minimum size in the free tier if we want to create more instances i have to terminate all the previous instances so that the 30gb will remain un used

![windows11](/images/readme/windows11.jpeg)
- Click `launch the instance`
- Scroll to bottom this page and Click on `View all instances`

![windows12](/images/readme/windows12.jpeg)

- Wait for changing the sate from `pending` to `Running `

![windows13](/images/readme/windows13.jpeg)
- Click on `Connect` if it's not visible go to `actions` there the `connect` option will be there

![windows14](/images/readme/windows14.jpeg)
- Go to `RDP Client` 
- There find the `Public DNS`
- There it will show `Get Password`

![windows15](/images/readme/windows15.jpeg)

- Upload Private File which is downloaded at the time of keypairs creations
- Click on teh `Decrypt the password` 

![windows16](/images/readme/windows16.jpeg)

- then you will be provided with the password

![windows19](/images/readme/windows19.jpeg)
- To connect the EC2 with the password usename and the dns we use third party service to connect local windows machine to virtual windows machine 
- The software to make this connection is `RDC` (`Remote desktop connection`)

![windows17](/images/readme/windows17.jpg)
- This software comes by default in the windows 
- In the computer put he `DNS`
- In Username put the `username`  

![windows18](/images/readme/windows18.jpg)
- Then click on the `connect` option
- Then it will ask for the password 
- Then put the `password` 
- Then click on `yes` 

![windows20](/images/readme/windows20.jpg)
- One the instance is launched you can close it and from where you have launched it from there only you can terminate it through instance state

![windows21](/images/readme/windows21.jpg)


## How to launch a Linux Instance

- Go to AWS Management console

- Select the server Asia Pacific (Mumbai) 

- - We are choosing Mumbai because it is nearest and the latency will be the lowest

- Go to the search bar and type `ec2` 

![searchMark](/images/readme/searchMark.jpeg)
- There check the availability zones of mumbai names as 
- - ap-south-1a
- - ap-south-1b
- - ap-south-1c
- - But the region is ap-south-1

## There are two ways to launch the EC2 instance
- By clicking Instance (running ) from the resouce panel 
- - This gives the running instances immediately
- By directly clicking the Instance button in the Same page

![launchInstanceRunning](/images/readme/launchinstancerunning.jpeg)

### Procedure
-  Click on the `Launch instance` button 

![launchinstance](/images/readme/launchInstancerunning2.jpeg)
-  Then there It will be aksing you the `name and tags `
- -  The tags are used to define the which types of instance it is

![windows1](/images/readme/windows1.jpeg)
-  Choose the `Application and Os Images (Amazon Machine Image)` 
- -  OS Images then find the Linux image then check for the free tier image 

![linux1](/images/readme/linux1.jpeg)

- `Key Pair (login)`

![windows6](/images/readme/windows6.jpeg)

![windows7](/images/readme/windows7.jpeg)

- `Network settings`

![linux2](/images/readme/linux2.jpeg)

## Web Server = Website

How we are going to install random web package 


