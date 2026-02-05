## Serverless Computing

In this section, I will be talking about what **serverless computing** is about. Not only that, but also **managed services**, **unmanaged services**, and **fully managed services** **Lambda**, **containers**, **Amazon EKS**, **ECS**, and so on.

So let start with serverless computing: this makes you deploy code or run your application without worrying about the underlying infrastructure. It is not that the computing does not have servers, that is why you should not worry. No, it is just that AWS will maintain that aspect for you while you focus on other aspects. So now let talk about the managed, unmanaged, and fully managed services.

### Managed Service
This means AWS is going to take care of most of the work for you, like setup, updates, scaling, security patches, and so on. Although you may still deal with configuration depending on the service, it comes with less control.

### Unmanaged Service
This means AWS is going to give you the infrastructure components for you to deal with, from customer data, firewall configuration, data encryption, maintenance, networking, and so on, which gives full control but comes with more aspects to maintain.

### Fully Managed Service
This means AWS takes care of every heavy aspect for you, meaning you don’t have to worry about servers or underlying infrastructure while you focus on development.

### Let talk about Lambda  
---
This is a serverless compute service that runs code based on events that occur, and you don't have to worry about servers because it automatically takes care of the underlying infrastructure. You can also scale up and down automatically based on requests at a time, and pay for only what you use.

Let imagine it like this: imagine a boss hires an assistant to answer only calls or messages on behalf of him because of the overwhelming work. You will agree with me that it is a flexible job because the assistant answers calls when someone is calling and can take a rest if no call enters, and that is also an event that occurs. It is the calls or messages that trigger the assistant to work.

Just look at Lambda like that: it is triggered to work based on events that occur and makes you pay only for the time you use it, without you managing servers. With this, you can use Lambda to host event-driven applications like gaming apps, news applications, e-commerce applications, and so on.

