# AWS-PROJECT
3-tier architecture 
This project is based on to create the production & Disaster Recovery environment in 3-tier architecture, using by the Domain which was purchased from the GoDaddy website, also giving the SSL certification. Cofigured and integrated such services and using some credentials by admin access for this. The production server contains some application contents, if it's suppose, the server region was down may be it was destroyed, we can recover the server data from the DR server which was created when the production server created. DR server was replicate the data what is in production server.
Created in the procedure to get server with configured and replicate the database
Created ACM,R53 then integrate both.
Security Groups to give access to traffic.
IAM roles
RDS setup with Subnet Group
EC2 instance creation for production and DR server with user description(to install httpd, mysql, linux extras and WORDPRESS). ELB setup with integration of those EC2 instance.
Integrate R53 & ELB under the Alias.
Created s3 buckets for production & DR.
Used CRONTAB for do some activity.
Transfering and made replicates between production and DR from DB to S3.
Finally, attached the ACM certificate in ELB for HTTPS port.
