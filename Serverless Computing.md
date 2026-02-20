# Serverless Computing + Containers (EKS / ECS / Fargate)

In this section, I will be talking about what **serverless computing** is about. Not only that, but also managed services, unmanaged services, and fully managed services, Lambda, containers, Amazon EKS, ECS, and so on.

So let’s start with serverless computing: this makes you deploy code or run your application without worrying about the underlying infrastructure. It is not that the computing does not have servers—of course it does! It is just that AWS will maintain that aspect for you while you focus on your work. 

#### 1. Unmanaged Service
This means AWS gives you the infrastructure components for you to deal with. From customer data, firewall configuration, and data encryption to maintenance and networking. This gives you **full control**, but comes with more things you have to maintain yourself.

#### 2. Managed Service
This means AWS takes care of most of the work for you, like setup, updates, scaling, and security patches. Although you may still deal with some configuration depending on the service, it comes with less manual work.

#### 3. Fully Managed Service
This means AWS takes care of every heavy aspect for you. You don’t have to worry about servers or the underlying infrastructure at all while you focus on development.

---

### Let’s talk about Lambda (Amazon Cloud Service)
This is a serverless compute service that runs code based on **events** that occur. You don't have to worry about servers because it automatically takes care of the infrastructure. It scales up and down automatically based on requests, and you only pay for what you use.

**Imagine it like this:** Imagine a boss hires an assistant to answer only calls or messages because he has too much work. You will agree that it is a flexible job because the assistant only answers when someone is calling and rests when there are no calls. That call is the "event" that triggers the assistant to work. 

Lambda is just like that: it is triggered by events and you only pay for the time it is actually working, without you managing any servers. You can use it for gaming apps, news apps, or e-commerce.

---

### Let’s move on to Containers 
First, I want you to imagine this like those **food flasks** where you can have your stew, bread, and egg all packaged in one place. A container comes with all the "packages" (code, settings, and tools) that allow your code to run in any stage of development.

**What is a "stage"?** Every app passes through three main steps:
1. **Development stage:** Getting everything together.
2. **Testing stage:** Checking for errors.
3. **Production stage:** Deploying it for everyone to use.

Sometimes, code works fine on a developer's laptop, but when they give it to a friend, everything starts falling apart! **Containers solve this.** Because the code is inside the "flask" with everything it needs, it works the same on any computer. It is lightweight, fast, and easy to manage.



### Scaling with Orchestration
When your app gets huge and you need more than one container, **Orchestration** gets you covered. It maintains multiple containers, scales them automatically based on demand, and does **load balancing** (sharing the traffic) for you.

---

### AWS Container Services

| Service | Description |
| :--- | :--- |
| **Amazon ECR** | The **Warehouse** for storing your container images. |
| **Amazon ECS** | The **AWS Manager** that runs your containers. |
| **Amazon EKS** | The **Manager** used for running Kubernetes containers. |
| **Fargate** | The **Serverless Engine** that runs containers without you worrying about servers. |

## What I cover in this document
- Serverless Computing
- Unmanaged Service
- Managed Service
- Fully Managed Service
- Lambda
- Containers
- Scaling with Orchestration
- AWS Container Services
