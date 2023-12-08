# To host a website on AWS:

1) Create an EC2 instance-
   - AMI: Amazon Linux
   - Security group: SSH, HHTP and HHTPS traffic should be allowed
     
2) Connect the instance and run following linux commands:
  - to install apache(httpd) webserver
    ```
    yum install httpd
    ```
  - to check the status of httpd
    ```
    service httpd status
    ```
    or
    ```
    systemctl status httpd
    ```
  - to enable httpd
    ```
    systemctl enable httpd
    ```
  - to start httpd
    ```
    service httpd start
    ```
    or
    ```
    systemctl start httpd
    ```
  - make a new directory(copy link of any website template from free-css.com)
    ```
    mkdir
    ```
  - to download a website template
    ```
    wget
    ```
    ```
    ls -lrt
    ```
    ```
    unzip
    ``` 
    ```
    cd
    ``` 
    ```
    ls -lrt
    ```
  - to transfer contents of the unzipped folder into the new directory
    ```
    mv * /var/www/html/
    ```
  - to access new directory
    ```
    cd /var/www/html
    ```
  - check if contents have been transferred
    ```
    ls -lrt
    ```
  - Now open the Public IP of the instance to see the website 
