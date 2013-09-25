Node JS Adaptations of AWS EC2 API Tools
========================================

Installation
------------
npm install aws-sdk optimist
npm install -g jsontool

Configuration
-------------
Create ~/.aws/default.json with content like:

    {
      "accessKeyId": "...",
      "secretAccessKey": "...",
      "region": "us-east-1"
    }

Usage
-----
./ec2-list-securitygroups --account production
./ec2-list-securitygroups --account production | ./format-securitygroups-friendly
./ec2-list-securitygroups --account production > groups.json
cat groups.json | ./format-securitygroups-friendly
