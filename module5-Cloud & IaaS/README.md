 <h1 align="center">module5-Cloud & IaaSπ₯³</h1>

β Introduction to Cloud & Infrastructure as a Service

β Setup server on DigitalOcean

β Deploy App on Droplet

β Create a Linux User
 
 ## Iaas => Infrastructure as a service (IaaS)
 
 Infrastructure as a service (IaaS) is a type of cloud computing service that offers essential compute, storage, and networking resources on demand, on a pay-as-you-go basis. 
 
 IaaS is one of the four types of cloud services, along with 
 - software as a service (SaaS), 
 - platform as a service (PaaS),
 - serverless.

### Introduction to Cloud & IaaS
β Watched video
### Setup a Server on DigitalOcean
β Watched video

β Demo executed

   - β Created a DigitalOcean account (Free Tier)

   - β Created a Droplet

   - β Configured Firewall rule to open port 22 for your IP address

   - β Connected to Droplet

   - β Installed Java on Droplet

### Deploy Application on Droplet 
β Watched video

β Demo executed

   - β Built Jar File with gradle

   - β Copied to remote Server (Droplet) 

   - β Run App on Droplet

   - β Configured Firewall Rule to open port 7071 to access App via browser

### Useful Links:
β You can clone this project: https://github.com/pmendelski/java-react-example
### Video - Create a Linux User 
β Watched video

β Demo executed

   - β Added User

   - β Added new User to sudo group

   - β Created .ssh folder with ssh key for new User 

## Best practices

β Security: Open ports only for specific IP addresses or ranges (Sources in 
Inbound Rules)

β Security: Do NOT use Root User. Create a new Linux user for every 
application and give it only the permission it needs to run that application.
