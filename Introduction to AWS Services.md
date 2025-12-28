## Understanding AWS Services

Now that I have covered what cloud computing is and other things related to it, at this stage an individual can choose a cloud provider and study their services.

Something interesting is that if you choose AWS Cloud and study it, you can still use the same knowledge for Google Cloud and other cloud providers. Some words may just change, but you don’t have to worry about that because the core concept remains the same.

Let us look at it this way: imagine you are working for a Toyota car company as a mechanical engineer. As time goes on, you stop working for them and start working for Honda. You are still a mechanical engineer, right? The brake, accelerator, and clutch are still in the same places in a car.
What may slightly differ are the guidelines and processes, but you are still a mechanical engineer.

In the same way, if you study AWS Cloud, you can still use that knowledge in other cloud provider environments.

I am preparing for the AWS Cloud Practitioner exam, so everything I will be talking about will be based on AWS Cloud. Some words may sound a little strange at first, and you may wonder, “What is that?” Don’t worry—we will understand what all these things are and how they work as we move forward.

In this section, I will be talking about one of the AWS services called ***Amazon EC2 (Amazon Elastic Compute Cloud)**. But you may be wondering, why did I have to study all this about cloud?

Imagine you are working in a pharmacy as a pharmacist. It is your job to know about different medicines and know which one to give to a customer based on their complaint.

Now, I want you to look at the AWS services that I will be discussing as medicines you must know. You need to understand how they work, when to use them, and how to explain their benefits to your CEO or anyone in the company who does not understand cloud computing.

That is what the AWS Cloud Practitioner exam is about, being familiar with these services. This does not make you a professional yet, but it gives you access to the knowledge (objectives) and the management console (theory) to understand how things work.



## What Is Amazon EC2 (Amazon Elastic Compute Cloud)?

In simple words, Amazon EC2 is a service that allows you to access compute resources such as CPU, memory, storage, networking, and more over the internet to run whatever  you need.

In other words, it means setting up a virtual server (compute) over the internet for your needs.

Under EC2, you can create something called an **EC2 instance**, which is a virtual compute that you can set up with just a click on the management console for your workload.

As time goes on, I will show how to set up an EC2 instance so we can see how it looks.

Let me use this example to clarify things more. Imagine getting a standing fan that is well packaged in a carton. Inside the carton, the fan is not yet assembled, but it is a product that is ready to use. When you get home, you have to set it up and configure it together for your needs.

See EC2 as a service offered by AWS Cloud that is ready to use, and the setup of that service is called an **EC2 instance**.

Something interesting again is that just the way you can go from a small standing fan to an industrial fan based on your needs and workload, that is how an EC2 instance also works.

You can add more to your instance to produce (more power) this is called **scaling up**.

In the same way, when you no longer need the industrial fan, you can stop using it and go back to your smaller fan. EC2 can also be **scaled down** (less power), or even turned on and off, and you are only going to pay for the time it runs.

## EC2 Instance Types

### 1. General Instance
This is very good for general purposes such as analyzing data, fast hardware usage, storing data, workloads, and more.


### 2. Compute Instance
This is very good for handling workloads because it provides more power. It is good for gaming, machine learning, and AI.


### 3. Storage Instance
This has the capacity to store large databases and handle workloads with high performance.


### 4. Memory Instance
This is good for analyzing databases with high performance.


### 5. Accelerated Instance
If you are looking for hardware with very good fast performance, accelerated hardware is the best.



## Instance Pricing 

Let us move forward a little bit to instance pricing, which is also very important to know as a beginner.

Spot, Savings, Reserved, On-Demand, Dedicated Host, Dedicated Instance

### On-Demand Instance
This is when you are paying for what you use. As I said in one of my documentation, if you use a service for 5 hours, you are only paying for those 5 hours, with no additional charges. This is good for startups and small businesses.

---

### Savings Instance
This creates a discount for any customer that stays dedicated to a particular service for one to three years. Imagine you are running an e-commerce website and you know you will need storage for at least three years. You will get a discount for that commitment.

---

### Reserved Instance
This is similar to a Savings Instance. If you commit to using an instance for one or three years in the same region, you will get a discount that is slightly higher than a Savings Instance, and the commitment level is more flexible than others.

---

### Spot Instance
Let me use an example to explain this. Imagine you have two phones but barely use your second phone. Your friend needs a phone and asks if they can use your second phone. You agree because you do not use it much, but you also tell your friend that you can take the phone back if you need it. Your friend agrees.

It is the same with Spot Instances. You are making use of AWS resources that are not currently being used, but AWS can interrupt you if they are needed, with a two-minute notice. You must agree to this condition. Spot Instances are very cheap and suitable for services that can be interrupted during processing.

---

### Dedicated Host
I will also use an example here. A Dedicated Host is like buying a standing fridge for yourself, no sharing, it is just for you. You can control what happens to it because it is dedicated to you.

Think of a Dedicated Host like buying a complete server rack for yourself for control and security reasons. It is expensive to set up and expensive to maintain.

---

### Dedicated Instance
Going back to the fridge example, this is when you are getting a small part of the fridge dedicated to you, like telling your younger sisters not to touch the meat in the upper part of the fridge because that section is reserved for you.

In the same way, a Dedicated Instance means you are getting a portion of a server rack for yourself and staying isolated from other AWS customers on the same server.

---

You may be thinking, does all this really sound like instance pricing? As mentioned earlier, we are like pharmacists who should explain to our customers: use this, use that, this one is cheap because of this, go with this if you are on a budget, and so on.


