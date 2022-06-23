# CloudDevops-Udacity-Project-2
Using Infrastructure as code to launch a web app 
## ND9991 - C2- Infrastructure as Code -
This folder provides the code for launching a web app using AWS CloudFormation. This was done to meet the requirements of my course work with Udacity.


### Dependencies
##### 1. AWS account
You would require to have an AWS account to be able to build cloud infrastructure.

##### 2. VS code editor
An editor would be helpful to visualize the image as well as code. Download the VS Code editor [here](https://code.visualstudio.com/download).

##### 3. An account on www.lucidchart.com
A free user-account on [www.lucidchart.com](www.lucidchart.com) is required to be able to draw the web app architecture diagrams for AWS.


### How to run the supporting material?
You can run the supporting material in two easy steps:
```bash
# Ensure that the AWS CLI is configured before runniing the command below
# Create the network infrastructure
# Check the region in the create.sh file
./create.sh myFirstStack network.yml network-parameters.json
# Create servers
# Check the region in the update.sh file
./update.sh mySecStack servers.yml server-parameters.json
# Delete stack after one after the other. Make sure you delete second stack before the first stack. 
#The second stack has dependencies on the first stack therefore the first cannot be deleted.
./delete.sh mySecStack
./delete.sh myFirstStack
```

For my work see http://secon-webap-1c7qkqov70d0r-1115334366.us-east-1.elb.amazonaws.com/
