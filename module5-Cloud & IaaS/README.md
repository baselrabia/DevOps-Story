 <h1 align="center">module5-Cloud & IaaS🥳</h1>

★ Introduction to Cloud & Infrastructure as a Service

★ Setup server on DigitalOcean

★ Deploy App on Droplet

★ Create a Linux User
 
 ## Iaas => Infrastructure as a service (IaaS)
 
 Infrastructure as a service (IaaS) is a type of cloud computing service that offers essential compute, storage, and networking resources on demand, on a pay-as-you-go basis. 
 
 IaaS is one of the four types of cloud services, along with 
 - software as a service (SaaS), 
 - platform as a service (PaaS),
 - serverless.

### Introduction to Cloud & IaaS
❏ Watched video
### Setup a Server on DigitalOcean
❏ Watched video

❏ Demo executed

   - ❏ Created a DigitalOcean account (Free Tier)

   - ❏ Created a Droplet

   - ❏ Configured Firewall rule to open port 22 for your IP address

   - ❏ Connected to Droplet

   - ❏ Installed Java on Droplet

### Deploy Application on Droplet 
❏ Watched video

❏ Demo executed

   - ❏ Built Jar File with gradle

   - ❏ Copied to remote Server (Droplet) 

   - ❏ Run App on Droplet

   - ❏ Configured Firewall Rule to open port 7071 to access App via browser

### Useful Links:
● You can clone this project: https://github.com/pmendelski/java-react-example
### Video - Create a Linux User 
❏ Watched video

❏ Demo executed

   - ❏ Added User

   - ❏ Added new User to sudo group

   - ❏ Created .ssh folder with ssh key for new User 

## Best practices

● Security: Open ports only for specific IP addresses or ranges (Sources in 
Inbound Rules)

● Security: Do NOT use Root User. Create a new Linux user for every 
application and give it only the permission it needs to run that application.
