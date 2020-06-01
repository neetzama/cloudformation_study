# Resource construction with AWS CloudFormation
It aims to automate the construction of the infrastructure environment.<br>
But I'm only talking about AWS CloudFormation here.<br>
[Click here][1] for an overview of the entire project.<br>

![cloudformation構成図](https://user-images.githubusercontent.com/60305322/82834520-55ffdc00-9efc-11ea-9f93-9ae6886cb934.png)

- Automatically create resources (EC2, RDS, ALB) using AWS CloudFormation.<br>
The block diagram is as above.
- The template file uses the yaml format.
- EC2Instance also performed advance preparation to link with Ansible and Serverspec.

## Requirements
- Region is Asia-Pacific (Tokyo : ap-northeast-1)
- RDS is PostgreSQL (EngineVersion 9.5.19)
- EC2 needs to be connected to the jenkins server via ssh, so it is generated from an AMI that has a common key.<br>
For instructions on how to create an AMI, see ["Requirements" here][1].

[1]: https://github.com/neetzama/jenkins_study
