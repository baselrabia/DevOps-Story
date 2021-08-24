<h1 align="center">module6-Nexus Artifact Repository Manager🥳</h1>


## Module Overview
★ Introduction to Artifact Repository Manager

★ Install and Run Nexus on Droplet

★ Nexus UI Tour

★ Repository Types

★ Publish Artifact to Nexus

★ Nexus API

★ Blob Store

★ Component vs Asset

★ Cleanup Policies


### Introduction to Artifact Repository Manager
❏ Watched video
### Install and Run Nexus on Droplet
❏ Watched video

❏ Demo executed

   - ❏ Installed Nexus on DigitalOcean Droplet

   - ❏ Created a new Linux User for Nexus

   - ❏ Changed permissions of Nexus executable and sonatype-work folder

   - ❏ Set Nexus configuration to run as Nexus User (nexus.rc file)

   - ❏ Started Nexus with Nexus User

   - ❏ Configured Firewall Rules to open port 8081 to access Nexus from 

### Useful Links:

● Nexus Download URLs: https://help.sonatype.com/repomanager3/download

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
❏ Watched video
### Repository Types
❏ Watched video 
### Useful Links:
- Nexus Repository Types: 
https://help.sonatype.com/repomanager2/configuration/managing-repositories
### Publish Artifact to Nexus
❏ Watched video
❏ Demo executed
   - ❏ Created new User on Nexus with permission to upload artifacts
   - ❏ Java Gradle Project: Build Jar File & Upload Jar File to Nexus
   - ❏ Java Maven Project: Build Jar File & Upload Jar File to Nexus

### Nexus API & Repository URLs
❏ Watched video
❏ Demo executed
   - ❏ Queried Repositories
   - ❏ Queried components of a repository
   - ❏ Queried assets of a component

### Blob Store
❏ Watched video
   - ❏ Demo executed - create a new blob store

## Check your progress... 3/3
### Component vs Asset
❏ Watched video
### Cleanup Policies
❏ Watched video
❏ Demo executed
   - ❏ Created new cleanup policy
   - ❏ Attached to a repository
   - ❏ Execute task manually

