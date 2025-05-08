---
hidden: true
noIndex: true
icon: server
cover: >-
  https://images.unsplash.com/photo-1605745341075-1b7460b99df8?crop=entropy&cs=srgb&fm=jpg&ixid=M3wxOTcwMjR8MHwxfHNlYXJjaHwyfHxEb2NrZXJ8ZW58MHx8fHwxNzQ1MDUzOTA2fDA&ixlib=rb-4.0.3&q=85
coverY: 46
---

# Compute Cluster (preview)

The Compute Cluster, once successfully materialized, will be a powerful network of servers that work together to provide cloud computing and self-hosted services for the Sheldon Bois. This will serve as a major upgrade to the current server infrastructure that runs the College Debt SMP while offering more power to run software in parallel.

In order to achieve this to the greatest extend, I invite everyone to take part in this new technological initiative. I'll explain more below to why this is more of a group project.

## Background

While plans for the College Debt SMP were still in conceptual phase, I ran across this one article that shows you how to run a FREE Minecraft server using a virtual machine from Oracle Cloud. If you're familiar with the IT scene, it's indeed the same company own by Larry Ellison, but they admittedly provide the whole foundation for the server to exist without having to charge any dime to you guys. The server, to this day, still use the same hardware from them.

Minecraft, unfortunately, is not a very CPU optimized game, so I have to almost give all of the server resources for the game to run as performant as possible. This prevents me from running anything additional at the same time, so that anyone playing won't be affected as much. With this consideration, I look into the possibility of expanding the current computation power.

To keep in short, there's two ways to increase a system's raw performance: either you upgrade the hardware to use faster components (vertical expansion), or you have more of the same hardware running in parallel (horizontal expansion). Oracle Cloud only give each user account a finite amount of allocation for their free tier, which I have maxed out. I can't create multiple account under myself without risking service termination, so this is where you guys can chime in.

By creating your own Oracle Cloud account, you will have free access to the same benefit as I do to run the server as of now. We can then link these virtual machines together to have all of them be coordinated as if they're one big system. As a gratitude for your involvement, I will give everyone access to it and provide administrative assistant as if it's collectively ours.

If anyone have access to any other machines that you would like to include in our server cluster, I'm also open to it. lol

## Technical facts

To help motivate the outcome of this project, I will describe the technical specification on how things are planned to work:

* Each Oracle Cloud account can claim up to 4 OCPU (equivalent to 4 cores, 4 threads) and 24 GB of ram for the free virtual machine. Think about when we scale this up to how many of us there are...
* Our sheldonbois.dpdns.org domain will serve as an entry point to access anything that we run on the server that has a web GUI
* For authentication purposes, you will need to log into your College Debt 365 account before you can access our hosted pages. You usually only need to do this one time for every new browser profile.
* Apps and software will be deployed as containers using Kubernetes (or Docker Swarm if I'm too lazy) as an orchestrator.

## Setup ahead of time

I will not be working on this plan until I'm officially out of the school year. For those who are already on break, you may get a head start on your part of this project. It should not take long. Let me know if you want to do it.
