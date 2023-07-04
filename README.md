# Deploy a Static Website on AWS EC2 

## DESCRIPTION: 
In this project, , an AWS EC2 instance (ubuntu) was launched then I deploy a MedicCare Health Specialist static website on the instance  through an apache webserver to the browser for visitor.


## STEPS
#### Launching EC2: 
- Choosed an AMI
- Choosed an Instance Type
- Configured the Instance
- Added Storage (default)
- Added Tags
  ![Tags](https://github.com/OK-CodeClinic/Deploy_Static_Website_on_AWS_EC2/assets/100064229/addc2d31-e45b-4250-94e3-272f94b422ea)

- Configure 
ecurity group, set some inbound rules to allow visitors to have access to my website
  ![SecurityGroup](https://github.com/OK-CodeClinic/Deploy_Static_Website_on_AWS_EC2/assets/100064229/fb0fe528-8e6c-4520-b302-3b4f4ee32862)


- Review, then launched.
  ![InstanceRunning](https://github.com/OK-CodeClinic/Deploy_Static_Website_on_AWS_EC2/assets/100064229/aa346a54-c6b9-406b-905a-fd890980bab3)



#### Connect:
- Open Gitbash
- Conncted via SSH client
- Run update
  ```sudo apt update ```
- Boom! EC2 was ready to use
  
  ![Connect](https://github.com/OK-CodeClinic/Deploy_Static_Website_on_AWS_EC2/assets/100064229/a0a6f4a8-69fe-404d-8a90-35b2d1c8772b)


#### Deployment:
- Logged in as a root user
- Install apache2 web server
  ```apt install apache2 -y```
- Start apache2 and check status
   ```systemctl start apache2``` ```systemctl status apache2```

  ![Deployment](https://github.com/OK-CodeClinic/Deploy_Static_Website_on_AWS_EC2/assets/100064229/7415bbc9-be77-4bb9-afef-81ea810d42a1)

  
- Now thata apache2 is running.
- Downloaded web artifact from tooplate.com
  ```wget https://templatemo.com/tm-zip-files-2020/templatemo_566_medic_care.zip```
- Unzip the artifact by running the unzip command
  ```unzip templatemo_566_medic_care.zip ```
- Copy all artifacts into the webserver directory
- Run on web browswer using the instance Ip address.


## OUTCOME
Server working fine, website working all fine.



![Outcome (2)](https://github.com/OK-CodeClinic/Deploy_Static_Website_on_AWS_EC2/assets/100064229/a2481d9c-6191-4fa7-a220-1c16a4a5089f)
![Outcome (1)](https://github.com/OK-CodeClinic/Deploy_Static_Website_on_AWS_EC2/assets/100064229/89fde1b2-acc2-4d76-a9f1-9b06ee464556)




## Author

- [Kehinde Omokungbe](https://www.github.com/OK-CodeClinic)

## Purpose
This is for leaning purpose only.
## Aknowledgment

Artifacts was downloaded from www.templatemo.com
