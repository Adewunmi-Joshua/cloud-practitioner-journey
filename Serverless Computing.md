## Serverless computing + containers / EKS / ECS

In this section, I will be talking about what **serverless computing** is about. Not only that, but also **managed services**, **unmanaged services**, and **fully managed services** **Lambda**, **containers**, **Amazon EKS**, **ECS**, and so on.

So let start with serverless computing: this makes you deploy code or run your application without worrying about the underlying infrastructure. It is not that the computing does not have servers, that is why you should not worry. No, it is just that AWS will maintain that aspect for you while you focus on other aspects. So now let talk about the managed, unmanaged, and fully managed services.

### 1. Managed Service
This means AWS is going to take care of most of the work for you, like setup, updates, scaling, security patches, and so on. Although you may still deal with configuration depending on the service, it comes with less control.

### 2. Unmanaged Service
This means AWS is going to give you the infrastructure components for you to deal with, from customer data, firewall configuration, data encryption, maintenance, networking, and so on, which gives full control but comes with more aspects to maintain.

### 3. Fully Managed Service
This means AWS takes care of every heavy aspect for you, meaning you don’t have to worry about servers or underlying infrastructure while you focus on development.

### Let talk about Lambda  (Amazon cloud service)
---
This is a serverless compute service that runs code based on events that occur, and you don't have to worry about servers because it automatically takes care of the underlying infrastructure. You can also scale up and down automatically based on requests at a time, and pay for only what you use.

Let imagine it like this: imagine a boss hires an assistant to answer only calls or messages on behalf of him because of the overwhelming work. You will agree with me that it is a flexible job because the assistant answers calls when someone is calling and can take a rest if no call enters, and that is also an event that occurs. It is the calls or messages that trigger the assistant to work.

Just look at Lambda like that: it is triggered to work based on events that occur and makes you pay only for the time you use it, without you managing servers. With this, you can use Lambda to host event-driven applications like gaming apps, news applications, e-commerce applications, and so on.

### Let move on to container
---

First, I want you to imagine this like those food flasks where you can have your stew, bread, and egg in them and package all what you need in one place. Same as container, it comes with all the packages that allow you to run your code in any stage of development.

What is stage, you may be thinking. Developers will be able to relate to this well, but let me explain. Every software or app we use today passes through the development stage, testing stage, and production stage.

1. Development stage: is the process of developing and getting everything together.

2. Testing stage: this is where the developer has to check for any error and make sure everything is working well.

3. Production stage: this is where the software or app is deployed and ready to be used by everybody.

But something funny is that everything may be working fine on my laptop without any worry in any of these stages, but when I give it to my friend or another developer to check it out on his computer, everything starts falling apart and not working.

That is where container comes in, because it comes with all what your code needs to run and work the same on any computer, and it is good for updating, managing, faster, and lightweight.

Now that you host with containers and everything is going fine, but suddenly the codebase becomes big, there is an increase in demand, and the setup becomes complicated and demanding more than one container.

Don’t worry, “**Scaling containers with orchestration**” will get you covered because it lets you maintain multiple containers and scale automatically based on demand. Not only that, it also does load balancing for you.


