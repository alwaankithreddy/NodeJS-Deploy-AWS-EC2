****Here, I deployed a Node JS application on the AWS EC2 Instance. ****

**Prerequisites**
1. I have cloned the entire project from the git-hub first.
    ```
    git clone https://github.com/verma-kunal/AWS-Session.git
    ```
2. Downloaded and installed NodeJs package.
   ```
   https://nodejs.org/en/
   ```
4. I have tested the application on my local machine to see if it's running. 
   ```
   npm install
   npm run start
   ```

**Create an EC2 Instance on AWS**

5. Create an IAM user with admin-level access and access type as password and connect through the Amazon console. 

6. Create an EC2 with configuration OS:Ubuntu, type:t2 micro, create a new key pair, and download the .pem
   
7. Connecting to the instance using ssh
    ```
    ssh -i instance.pem ubunutu@<IP_ADDRESS>
    ```
8. Update the ubuntu packages
   ```
   sudo apt update
    ```
9. The latest version of Ubuntu is already getting git and installed, but we need to make sure running the below command and should give output something like this `git version 2.39.3`
    ```
    git -v
    ```
10. Install NodeJS and `npm` -  [Guide by DigitalOcean](https://www.digitalocean.com/community/tutorials/how-to-install-node-js-on-ubuntu-22-04)

    **Deploying the NodeJS app on EC2**

11.  clone the Repo
    ```
    git clone https://github.com/verma-kunal/AWS-Session.git
    ```
12. Install npm (it installs all the dependencies)
    ```
    npm install
    ```
13. Start the project
    ```
   npm run start
   ```


**HURRAY, WE DEPLOYED AN NODEJS APPLICATION ON AWS EC2C**

Note: We will need to edit the inbound rule of the security group on the ec2 instance and allow port 3000. 
    
    
    
