# Write-up Template

### Analyze, choose, and justify the appropriate resource option for deploying the app.

*For **both** a VM or App Service solution for the CMS app:*
- *Analyze costs, scalability, availability, and workflow*
- *Choose the appropriate solution (VM or App Service) for deploying the app*
- *Justify your choice*

Article CMS project is a light weighted Web project combination of 

a) SQL server - To store the users and post tables

b) Storage account - To Store the pictures

c) Flask Web application - Small python based web applications

d) MSAL & Active Directory - For the standard authentication and logging activities

**My preference is to go with the Web Applications over VM**

**VM (Vurtual Machine):**
Generally, VM cost more(compared to Web Apps) and is specially used when custom software applications are to be installed.
This application is not required to have full control of underlying operating systems.

**WebApps:**
_Web Apps support a maximum of 14 GB of memory and 4vCPU cores. That is enough for our application. 
Cost is cheaper compared to VM.
Our app is a nonproduction use and doesn't have any sensitive information._
### Assess app changes that would change your decision.

*Detail how the app and any other needs would have to change for you to change your decision in the last section.*
  If we have highly secured data(Government or confidential)  to deal with recommended to go with VM as compared to web apps.
  If we need a production app with a higher user base across regions I would go with VM.
