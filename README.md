#!/bin/bash
 yum install update -y
 yum install ruby -y
 yum install jq -y
yum install httpd

 cd /home/ec2-user
 wget https://aws-codedeploy-us-east-1.s3.amazonaws.com/latest/install
 chmod +x ./install
 ./install auto
 service codedeploy-agent start
