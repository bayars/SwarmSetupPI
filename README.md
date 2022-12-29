# SwarmSetupPI

## Hardwares
In my case, I have these hardware,
+ 3 - raspberry pi zero 2w
+ 1 - raspberry pi 3
+ 1 - 2TB Hard Disk
+ 1 - 500GB Hard Disk

## My Design
I planned use these hardwares for homelab. I will serve to my family members to use in the personal life. This ansible repository uses docker swarm to create and configure docker containers automatically. 

I am serving these applications,
+ nextcloud 
+ wireguard
+ samba
+ redmine
+ plex
+ drone CI/CD

As you would expect, one raspberry pi 3 won't enough to serve these applications. I am adding the three zero 2w's as worker nodes to manager node (raspberry pi 3). I tested with three different operation at the same time on the applications. I guess they can run more containers. I didn't see any performance problems.

These node management runs with ansible inventory grouping. (Look the hosts file)

Currently, I am using my another private personal server repository on github. That repository contains the docker compose files. I may open this repository to public in the future.
