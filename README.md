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
- Configure Security group, set some inbound rules to allow visitors to have access to my website
- Review, then launched.


#### Connect:
- Open Gitbash
- Conncted via SSH client
- Run update
  ```sudo apt update ```
- Boom! EC2 was ready to use


#### Deployment:
- Logged in as a root user
- Install apache2 web server
  ```apt install apache2 -y```
- Start apache2 and check status
   ```systemctl start apache2``` ```systemctl status apache2```
- Now thata apache2 is running.
- Downloaded web artifact from tooplate.com
  ```wget https://templatemo.com/tm-zip-files-2020/templatemo_566_medic_care.zip```
- Unzip the artifact by running the unzip command
  ```unzip templatemo_566_medic_care.zip ```
- Copy all artifacts into the webserver directory
- Run on web browswer using the instance Ip address.


## OUTCOME
Server working fine, website working all fine.





## Author

- [Kehinde Omokungbe](https://www.github.com/OK-CodeClinic)

## Purpose
This is for leaning purpose only.
## Aknowledgment

Artifacts was downloaded from www.templatemo.com
