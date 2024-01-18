# CloudFormation for Installing Execution & Consensus Client on EC2

Make sure to import env **AWS_ACCESS_KEY_ID**, **AWS_SECRET_ACCESS_KEY**, **AWS_DEFAULT_REGION** before running the **execution_client.yml** 

aws cloudformation deploy --template-file execution_client.yml --stack-name demo --capabilities CAPABILITY_IAM

# How the Infrastructure Looks Like

We will be having 2 Instances one is for Execution & Consensus Client and other is Monitoring Stack responsible for Scrapping metrics as well as alerting the notification to any channel as discord etc!

And On the Monitoring stack for further security, we can have login with org Email rather than having the static username and password and it will be behind the nginx server as web-server proxy!!
