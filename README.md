# AWS: Cloud Server

Practice auto-deploying using Elastic Beanstalk

## Labs 16

### Author: Mike Pace

### Links and Resources

-[Repo](https://github.com/catdude2000/cloud-server)  
[Deployed from EB Console](http://aws-lab16-roledone-env.eba-4idn32fa.us-east-2.elasticbeanstalk.com/)
[Deployed from CLI](http://express-server-aws.eba-xiyp385e.us-east-2.elasticbeanstalk.com/)

### Collaborators  

John Cokos, Codefellows

#### Running the app

clone repo  
`npm i`  
Follow Below

## Overview

Creating an application with the Elastic Beanstalk GUI
Choose NodeJS as your platform
Create and upload a .zip file with your application source code
Do not include node_modules or package-lock.json
This will create your application and environment in one step, giving you a full GUI from where you can manage the app

reating an application using the command line only
First, ensure that you've installed the AWS CLI and the aws eb command line utilities.

eb init - Initializes your folder as an Elastic Beanstalk application
Choose your region (us-west-2)
Choose [Create new Application]
Note: If you already have an application, you could also choose that to connect
Answer the other questions as appropriate
Choose Node.js at the correct version
eb create my-environment-name - Create an "environment" for your app to reside in
eb deploy to deploy your new application to your new environment
You'll also use this whenever you make code changes
You can then use some other eb commands to manage your apps

eb open to open your app in the browser
eb list to get a list of apps
eb ssh to ssh (login) to one of your apps
eb health to get a health check on your environments
