# Serverless Computing + Containers (ECS / EKS / Fargate)

In this section, I will be talking about what **serverless computing** is about. Not only that, but also **managed services**, **unmanaged services**, and **fully managed services**, including **Lambda**, **containers**, **Amazon EKS**, **ECS**, and more.

## Understanding Service Levels

1. **Unmanaged Service**
This means AWS gives you the infrastructure components, but you deal with everything else: customer data, firewall configuration, data encryption, maintenance, and networking. This gives you **full control** but comes with much more to maintain.

2. **Managed Service**
This means AWS takes care of most of the work for you, like setup, updates, and security patches. Although you may still deal with some configuration and scaling settings, it comes with less manual work but also less control.

3. **Fully Managed (Serverless) Service**
This means AWS takes care of every heavy aspect for you. You don’t have to worry about servers or underlying infrastructure at all. You focus entirely on development while AWS handles the scaling and availability.

---

## Amazon Lambda (Serverless Compute)
Lambda is a serverless compute service that runs code based on **events**. You don't have to worry about servers because AWS automatically takes care of the underlying infrastructure. It scales up and down automatically based on demand, and you **pay only for the time your code is running**.

**The Assistant Analogy:**
Imagine a boss hires an assistant to answer calls only when they come in. It is a flexible job because the assistant works when the phone rings (**an event**) and rests when it doesn't. You only pay the assistant for the time spent on the phone. 

Just like that, Lambda is "triggered" by events (like a file upload or a website click). It is perfect for event-driven applications like gaming apps, news alerts, or e-commerce processing.

---

## Containers (The Food Flask )
Imagine a food flask where you package your stew, bread, and egg all in one place. A **Container** is similar—it packages your code with every library and setting it needs to run.

### Why do we need them?
Software goes through different stages: **Development** (building it), **Testing** (checking for errors), and **Production** (ready for users). 

A common problem is when code works fine on a developer's laptop but "breaks" when moved to a different computer. This is where containers come in! Because everything the code needs is inside the "flask," it works exactly the same on any computer. They are lightweight, fast, and easy to manage.

### Container Orchestration
When your app grows and you need hundreds of containers, you need **Orchestration**. This is a system that manages all your containers, handles **Scaling** (adding more when busy), and **Load Balancing** (distributing traffic so no container gets overwhelmed).

---

## AWS Container Services

| Service | Description | Simple Role |
| :--- | :--- | :--- |
| **Amazon ECR** | Elastic Container Registry | **The Warehouse:** Used for storing and managing your container images. |
| **Amazon ECS** | Elastic Container Service | **The AWS Manager:** A highly scalable, high-performance way to run containers. |
| **Amazon EKS** | Elastic Kubernetes Service | **The Open-Source Manager:** Used for running Kubernetes containers on AWS. |
| **AWS Fargate** | Serverless Container Engine | **The Hands-Off Engine:** Allows you to run containers (ECS or EKS) without managing any servers. |
