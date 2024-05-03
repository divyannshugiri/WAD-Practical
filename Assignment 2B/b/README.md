What is Docker?

Docker is a tool designed to make it easier to create, deploy, and run applications by using containers. Containers allow a developer to package up an application with all of the parts it needs, such as libraries and other dependencies, and ship it all out as one package.

![image](https://github.com/divyannshugiri/WAD-Practical/assets/154437803/a25d38f5-bc73-437b-b169-17b691910c48)


Let’s say you need to build an application. That could be the next Facebook, Pandora, Amazon, Youtube, Spotify, or whatever. To make that application available to the public, you need someplace to host it. In the past, you would need to build your own computer and set up a dedicated web service called “server,” which is basically a computer dedicated for hosting websites or web services. The other option would be deploying that application to hosting companies such as 1&1, GoDaddy, Geocity, etc.

Then, the age of “cloud” came in. A company like Amazon Web Service (AWS) became very good at hosting your application through their own “data center,” — a collection of servers.

![image](https://github.com/divyannshugiri/WAD-Practical/assets/154437803/e383b4b4-7310-4de4-b217-e44d54b51a01)

Unlike web hosting services, these companies adopted a concept called “virtualization,” meaning that the hardware resources can be broken down even further through software functionality and provide resources more optimally to customers who need them.

This is why “cloud computing” is known as “utility computing” because you only pay for the services you use, instead of setting up the entire server for your own use. This is generally more cost efficient for both yourself and for the hosting company, not to mention it is more optimized for performance.

But even traditional cloud computing cannot avoid one thing — heavy Operating System usage. The operating systems refer in this case are Microsoft Windows, Linux (RHEL, Ubuntu, Fedora, etc), and MacOS. These OSs are large in size and can easily go over 1 Gigabyte, also known as “OS image.”

However, your application may only have an approximated size of 300 Megabytes to start with. So, why would you want a “virtual machine”, which is a virtualized environment resulted from virtualization, that has the size of 1 GB + when your application is much much less than that?

That’s where the concept of “container” comes in to fix that. Docker does it in the following way. Instead of hosting each operating system per each application, some common resources can be shared, and there is something called “docker engine,” which sits on top of an Operating System as shown below.

![image](https://github.com/divyannshugiri/WAD-Practical/assets/154437803/13c3f606-d918-443f-9605-87525607df48)

As you can see from the figure above, you can visually observe how the “app number” became much less with the use of a container. In one way, this is a very simple solution, nothing more than introducing another layer between OS and applications to optimize resource usages and reduce the need for redundant operating systems.

However, this is a breakthrough for application development because this level of abstraction is exactly what enterprise companies and individual developers needed — less hassle to “provision” giant virtual machines but only get minimum “containers” essential to host their applications.

![image](https://github.com/divyannshugiri/WAD-Practical/assets/154437803/553f0a98-dc65-478f-8b01-c427a244de29)

The result from adopting docker, or container, is that application can be deployed or undeployed faster, start and stop faster, change to another “image” faster, process and do many things faster.
