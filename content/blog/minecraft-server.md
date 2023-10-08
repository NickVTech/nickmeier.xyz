---
title: "Minecraft For My Brother"
date: 2023-06-14T12:12:43-04:00
draft: false
thumbnail: /images/blog/minecraft/Minecraft.webp
---


![Minecraft](/images/blog/minecraft/Minecraft.webp)

Its June 14, 2023. River, my younger brother, asked me if I was busy. I said "depends." He had been wanting to play video games with me since I had been home from college. The only problem was that I quit video games. The minecraft update "Trails and Tails" just came out, and he wanted to spend some quality time with me. I said yes, but first, on only one conditon. I needed to make the server myself.

Previously, before I had gone to college, I would buy some online hosting. There are many webistes, that sell very cheap server hosting. It has always amazed me how they could build a website that did all this. On the backend, I understood something was going on. I didn't want to rent a server this time.

I knew it was possible, so I put on my thinking cap and got to work...

![computer](/images/blog/minecraft/minecraftwithfrens.png)
## Gathering the materials

I thought about the materials needed to get this server running. About a year beforehand, my Mom told me her work was getting rid of a few computers, and was asking me and the brothers if we wanted one. These were old computers, used by her work, for simple tasks. I told her I would gladly take them off her hands. I didn't know what I was going to do with them, but I knew eventually I would find them useful. I am very lucky I had done that, because now I had the reasources for a free server. I connected some old wires up, and luckily my second monitor has a VGA port on the back, so I could use the same display for both my server and computer. I scrapped some of the old parts out of each of the computers, and used the best case in order to frankestien together a very capable server.


## The Recipe

I watch a lot of youtube, as you can see from my [youtube section](/youtube). I had previously followed a youtube channel I strongly recommend. I have his channel linked below. 

- [Hardware Haven](https://www.youtube.com/@HardwareHaven).

{{< youtube id="eIHiRW4QH6I" width="560" height="315" >}}

##### Warning, the following is my attempt to explain technical insight, please skip to next section if you don' care as much.

After watching the video, I understood a little bit more about how I would begin to build the server. Prior to this, I had little experience in networking. Previously, in 6th grade, I had made a mincraft server before. The only problem was I did not know how to port forward, or what that even was. Through the years, I had learned about why I actually needed to port forward. This included how machines communicated over ports, permissions, and what the concept of a firewall actually is. 

Definig the problem is 99% of the solution. To understand which materials I needed, would solve the problem itself. I didn't really know what to do, and what I needed, but by gathering the correct materials would mean that I knew how to solve this.

- #### Hardware
    - Didn't want to get out the specs.
- #### Ubuntu Server
    - This handles the operatinng system of the computer. I use it, to privde the foundation for running Docker containers. It manages the system-level resources.
    - Manages CPU, RAM, and storage. It ensures there is hardware available for Docker containers to run effectively.
    - [link](https://ubuntu.com/server)
    - ![computer](/images/blog/minecraft/ubuntuserver.png)
- #### Docker
    - What is Docker? Ok, docker is really cool because it allows you to run different servers on one operating system. Docker just really leverages the information provided by the operating system, to dynamically allocate reasources to different "containers" (servers). This is a foundational feature, and it provides other benefits that stem from this.
    - I wanted to use docker, because I could then also use this server for other applications as well. I really wanted to save my limited reasources, and I was told learning docker is really important. I can see the problems it solves, and how amazing the software is.
- #### Minecraft Container
    - The link below is the repository for the minecraft container. It has nice documentation, so give it a look if you're curious.
    - [Link](https://github.com/mtoensing/Docker-Minecraft-PaperMC-Server)


![computer](/images/blog/minecraft/computer1.JPG)
![computer](/images/blog/minecraft/computer2.JPG)
## Crafting

![computer](/images/blog/minecraft/gpu.JPG)

![computer](/images/blog/minecraft/minecraftwithfrens.JPG)

## Port Forwarding

##### Why Do We Need Port Forwarding for Minecraft?

Imagine your home's internet connection as a guarded castle gate, and inside the castle is your Minecraft server. Your friends from other villages (or networks) want to visit your castle and play Minecraft with you. To allow them in, you need to tell the guards (your router) to let visitors come to a specific door (port) where the Minecraft server is.

This process of telling the guards to allow visitors through a specific door is what we call "port forwarding." It lets your friends connect to your Minecraft server from their homes.


##### Setting Up Port Forwarding for Minecraft:

    1. Log in to Your Router: Open a web browser and type in your router's IP address, commonly 192.168.1.1 or 192.168.0.1.

    2. Navigate to Port Forwarding: Find the section named "Port Forwarding", "Virtual Server", or something similar.

    3. Create a New Rule: Forward the external port 25565 to the internal IP address of your device (the one running the Minecraft server) also on port 25565.

    4. Save and Restart: After adding the rule, save the changes. You might need to restart the router for the changes to take effect.


## Reflection

![computer](/images/blog/minecraft/reflection.jpg)
Looking back, I think this was more than just gaming. It was a venture into the heart of networking, getting hands on with Docker, and rekindling the memories of my 6th-grade self. Some things stay timeless, like the joy of sharing a game sesh with my younger brother, remain timeless. As we ventured into the "Trails and Tails" update, I realized that some trails in life are worth revisiting, especially when they lead to cherished memories. As for the future, I'm excited to explore more avenues in the tech realm, leveraging my newfound knowledge. But more importantly, I eagerly await many more gaming sessions with River, because sometimes, it's the simple joys that truly matter.