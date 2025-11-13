**#Postman API Automation Integration with Github actions#**

This repository a POC for integrating postman tests with github actions.Tests are written in postman and are executed in VM with the help of newman and newman-reporter-htmlextra.
Github actions will trigger the  project execution on every push to the main branch.You can also execute the project manually using workflow_dispatch.The projects run on a scheduled 
time with the help of the cron job.

The html report is archived and kept in the artifact section for the team to download it.Along with that they can view the report directly from the github page https://github.com/Sudeshna236/PhoenixInwarrantyFlow
The latest report is called to the team members using GMAIL SMTP.

**##About Me##**

My name is Sudeshna Bangalore. I have 5 years experience in Automation Testing.My Skill sets includes UI automation with Selenium Web driver, Cypress, Playwright and for
APItesting I use Rest Assured and Postman. You can connect with me over:(https://www.linkedin.com/in/sudeshna-supraja/)

**##Testing Coverage##**

1.Happy flow

2.Negative Testing

3.Edge case testing

4.Token testing

5.Data Driven Testing with CSV

6.Schema Validation

7.Secrets management with Github Secrets

**##Tech Stack##**

1.Postman

2.NodeJs

3.Newman

4.Newman-Reporter-HTMLextra

5.Github Actions

6.Gmail SMTP

7.Github pages

8.CSV for Data Driven Testing

9.AWS-EC2 Instance for Self hosted github runner.

## Github pages ##
you can directly view the latest test report of the postman test at the Github page link : https://github.com/Sudeshna236/PhoenixInwarrantyFlow


## HTML report ##
Report will be created in newman folder
![Postman Report](https://github.com/Sudeshna236/PhoenixInwarrantyFlow/blob/Static-Content/Newmanreport.png)

## Project Structure ##


PhoenixInwarrantyFlow

```
PhoenixInwarrantyFlow
├─ demo.txt
├─ InwarrantyFlowCollection.postman_collection.json
├─ QA.postman_environment.json
└─ testdata.csv

```

## How to run the project? ##

You can run the project on your local system for that:

1.Clone the project on local system :https://github.com/Sudeshna236/PhoenixInwarrantyFlow.git

2.Install nodejs and npm :https://nodejs.org/en

3.Install newman using ``` npm install -g newman ```

4.Install newman-reporter-htmlextra : ```npm install -g newman-reporter-htmlextra ```

5.run the newman command:
					
          newman run InwarrantyFlowCollection.postman_collection.json \ 
         -e QA.postman_environment.json \
         -d testdata.csv \
         -r cli,htmlextra \
         --reporter-htmlextra-export ./newman/index.html 
				










