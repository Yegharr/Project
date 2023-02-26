Using terraform create
autoscaling group with launch template which should  contain user data as well
user data
#!/bin/bash
# Use this for your user data (script from top to bottom)
# install httpd (Linux 2 version)
yum update -y
yum install -y httpd
systemctl start httpd
systemctl enable httpd
echo "<h1>Hello World from $(hostname -f)</h1>" > /var/www/html/index.html
ALB in front of autoscaling group which will listen 80 port and pass requests to autoscaling group instances