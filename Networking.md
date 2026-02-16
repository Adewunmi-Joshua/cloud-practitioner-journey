# Cloud Networking 

Networking is one of the very important parts in the cloud learning journey and an interesting part also. So let's dive in and talk about VPC (Virtual Private Cloud), Subnet, public subnet, and private subnet and more.

### What Is Cloud Networking?
Cloud networking is the process of designing, managing, and securing network resources in the cloud to allow communication between applications, users, and services without managing physical infrastructure.

---

### What Is VPC (Virtual Private Cloud)?
This allows you to have a private section in the cloud virtually and stay isolated from other customers to launch your resources.

**VPC Analogy**
Imagine you are living in a big compound with your family. Even though you share the same environment as others, you have your own fenced-in section. You are the boss of this section. You decide who comes in and what happens inside.

**The Internet Gateway (IGW):** Every compound needs a **Main Gate**. In AWS, this is the Internet Gateway. Without this gate, your VPC is locked shut no one can come in from the internet, and you can’t get out.

## Important of VPC
1. Increase security
2. Save Time
3. Conrol enviroment


---

### What Is a Subnet?
This allows you to arrange your resources into **public** and **private** sections. It is used to isolate your resources so you can share some publicly and keep others hidden.

* **Subnet Analogy (The House):**
Let’s go back to your house in the compound. Imagine your house has different rooms

1. **Public Subnet (The Parlor):**
You will agree with me that if a visitor arrives, the first place they are allowed to sit is the parlor. It’s public for everybody. In the cloud, this is where you put things like your **Website Frontend** where visitors can sit, change the TV channel, and feel relaxed.

2. **Private Subnet (The Bedroom):**
Your bedroom is not for the public to enter because it contains your personal belongings and you need privacy. In the cloud, this is where we group things like **Databases, storage, and backend servers.** Just like your room, it is a restricted section.

**How they talk to each other:**
Even though your room is private, you can still give access to trusted people (like developers or engineers). Also, your "Parlor" (the website) can talk to your "Bedroom" (the database) to get information, but the visitor at the main gate cannot go straight into your bedroom!

---

### Staying Secure: The Security Guard
To make your house even safer, AWS has two types of "guards":

* **Network ACL (NACL):** Think of this as a **Security Guard at the gate of the house**. He checks everyone coming into the parlor or the bedroom area. (This works at the **Subnet** level).
* **Security Groups:** Think of this like a **Bouncer standing at the door of a specific room**. He checks the ID of anyone trying to enter that specific door. (This works at the **Instance** level).


# Ways to Connect to the AWS Cloud

Let talk about some other ways to connect to the AWS Cloud.

We have AWS Client VPN, AWS Site-to-Site VPN, AWS PrivateLink, and AWS Direct Connect.

---

## AWS Client VPN

AWS Client VPN: This is a type of networking service that allows organisations to connect their remote workers and allow them to access their cloud resources in a safe way, and it is a fully managed elastic VPN service that automatically scales up and down based on user demand, which means you don't have to worry about any infrastructure layer.

Let imagine it like this: you have a company and most of your workers are spread across the globe, but they need to access your company AWS resources in the cloud, which you will want them to access in a safe way. That is where AWS Client VPN comes in because that is what it does.

---

## AWS Site-to-Site VPN

AWS Site-to-Site VPN: This is good if a company wants to connect their on-premises data center to their AWS Cloud resources in a safe way, and it is good to connect two branch offices together and allow them to access the company cloud resources, and the data stays encrypted during the process and safe.

---

## AWS PrivateLink

AWS PrivateLink: Some companies prefer a simple and private way to connect without using AWS Client VPN or AWS Site-to-Site VPN. If you are that company, AWS PrivateLink is for you because it is a highly available and scalable network that enables private connectivity between Amazon Virtual Private Clouds (VPC), AWS services, and on-premises networks without using public IPs, internet gateways, NAT devices, or firewalls.

Even though the preceding connections are highly available and scalable, traffic jams are possible because you’re using the same connection as other clients. That's why for some use cases, you might need a dedicated private connection with a lot of bandwidth.

---

## AWS Direct Connect

AWS Direct Connect: This allows you to have a dedicated connection from your organisation to AWS.

I don’t know if you have seen where they run fiber optic cables through the ocean to different locations and pass through different countries. That is similar to how Direct Connect looks like. However, it does not literally run fiber directly from your office to AWS by itself. It connects through AWS Direct Connect locations, which then provide a private dedicated connection from your organisation to your AWS resources.

