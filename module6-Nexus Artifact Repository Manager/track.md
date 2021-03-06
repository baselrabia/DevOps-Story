<h1 align="center">module6-Nexus Artifact Repository Managerπ₯³</h1>


## Module Overview
β Introduction to Artifact Repository Manager

β Install and Run Nexus on Droplet

β Nexus UI Tour

β Repository Types

β Publish Artifact to Nexus

β Nexus API

β Blob Store

β Component vs Asset

β Cleanup Policies


### Introduction to Artifact Repository Manager
β Watched video
### Install and Run Nexus on Droplet
β Watched video

β Demo executed

   - β Installed Nexus on DigitalOcean Droplet

   - β Created a new Linux User for Nexus

   - β Changed permissions of Nexus executable and sonatype-work folder

   - β Set Nexus configuration to run as Nexus User (nexus.rc file)

   - β Started Nexus with Nexus User

   - β Configured Firewall Rules to open port 8081 to access Nexus from 

### Useful Links:

β Nexus Download URLs: https://help.sonatype.com/repomanager3/download

### Useful Commands:

```bash
apt update
apt install openjdk-8-jre-headless
apt install net-tools
cd /opt
wget https://download.sonatype.com/nexus/3/latest-unix.tar.gz
tar -zxvf latest-unix.tar.gz
adduser nexus
chown -R nexus:nexus nexus-3.28.1-01
chown -R nexus:nexus sonatype-work
vim nexus-3.28.1-01/bin/nexus.rc
run_as_user="nexus"
su - nexus
/opt/nexus-3.28.1-01/bin/nexus start
ps aux | grep nexus
netstat -lnpt
```
## Check your progress... 2/3

### Nexus UI Tour
β Watched video
### Repository Types
β Watched video 
### Useful Links:
- Nexus Repository Types: 
https://help.sonatype.com/repomanager2/configuration/managing-repositories
### Publish Artifact to Nexus
β Watched video

β Demo executed
   - β Created new User on Nexus with permission to upload artifacts
   - β Java Gradle Project: Build Jar File & Upload Jar File to Nexus
   - β Java Maven Project: Build Jar File & Upload Jar File to Nexus

### Nexus API & Repository URLs
β Watched video

β Demo executed
   - β Queried Repositories
   - β Queried components of a repository
   - β Queried assets of a component

### Blob Store
β Watched video

β Demo executed 
   - β create a new blob store

## Check your progress... 3/3
### Component vs Asset
β Watched video
### Cleanup Policies
β Watched video

β Demo executed
   - β Created new cleanup policy
   - β Attached to a repository
   - β Execute task manually

