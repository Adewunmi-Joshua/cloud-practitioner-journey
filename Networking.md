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


---

### What Is a Subnet?
This allows you to arrange your resources into **public** and **private** sections. It is used to isolate your resources so you can share some publicly and keep others hidden.

* **Subnet Analogy (The House):**
Let’s go back to your house in the compound. Imagine your house has different rooms

1. **Public Subnet (The Parlor):**
You will agree with me that if a visitor arrives, the first place they are allowed to sit is the parlor. It’s public for everybody. In the cloud, this is where you put things like your **Website Frontend** where visitors can sit, change the TV channel, and feel relaxed.

2. **Private Subnet (The Bedroom):**
Your bedroom is not for the public to enter because it contains your personal belongings and you need privacy. In the cloud, this is where we group things like **Databases, storage, and backend servers.** Just like your room, it is a restricted section.


More is coming.
