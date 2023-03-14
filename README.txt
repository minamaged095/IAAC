1. Test URL:

http://proje-loadb-1k5b6cgtc7esg-951133723.us-west-2.elb.amazonaws.com/

2. Commands to run the stacks:

aws cloudformation create-stack --stack-name project-2-network --template-body file://network.yml  --parameters file://network-parameters.json --region=us-west-2

aws cloudformation create-stack --stack-name project-2-servers --template-body file://servers.yml  --parameters file://servers-parameters.json --region=us-west-2 --capabilities CAPABILITY_NAMED_IAM
