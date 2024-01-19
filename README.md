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
8.  
