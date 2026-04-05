# Storage ( AWS )

In this section I will be discussing what cloud storage is, types of cloud storage, Amazon S3, S3 storage classes and so on.

So let get started.


## What is Cloud Storage

This is a kind of service that allows users to access data, manage data, and save data over the internet instead of them having a physical storage hard drive themselves, which is going to cost a lot and require maintenance. 

Another interesting thing is that you are only going to pay for what you use, which is one reason big organisations love to use it.

---

## Type of Storages

# Block Storage

This is a type of high performance storage that stores data in fixed block sizes that attach to your EC2 instance when created, just like a hard drive, and provides persistent and low latency storage.

Under block storage we have two types of storage:

- Amazon EC2 Instance Store  
- Amazon Elastic Block Store

---

### Amazon EC2 Instance Store

This is a storage that attaches to your EC2 instance when hosted that comes with disk types and sizes depending on the EC2 instance.

But it has its own downside because once you stop or terminate the EC2 instance the data is gone. The data stored in it is only active when your EC2 instance is running.

So it is good only for temporary storage purposes like:

- Cache  
- Buffering  
- Scratch files and so on  

If you are looking for something that comes with storage that is cost effective and fast, then Amazon EC2 Instance Store is the right choice.

---

### Amazon Elastic Block Store

Amazon Elastic Block Store is another type of block storage provided by AWS that allows you to create storage volumes and attach them to your EC2 instance.

Unlike EC2 Instance Store, Amazon Elastic Block Store keeps your data even if you stop your EC2 instance. This means the storage is persistent and reliable.

It works very similar to a traditional hard drive that you attach to a server, but the difference is that it runs in the cloud and can scale based on your needs.

Amazon Elastic Block Store is commonly used for things like:

- Databases  
- File systems  
- Applications that require persistent storage  

Another good thing about Amazon Elastic Block Store is that it allows you to create snapshots of your volumes which can be used for backup and recovery purposes.

This makes it a reliable storage option when running applications that require consistent and durable storage.

## Let’s talk about EBS Snapshot

An EBS snapshot is a point-in-time backup of an EBS volume that can be used to restore data or create new volumes later.

To make this more clear, let’s look at it like this.

An EBS volume, which is Elastic Block Store volume, is just like a hard drive in your computer/system.

An EBS snapshot is like taking a picture of the hard drive at a particular moment for backup in case of any disaster that occurs. AWS stores these snapshots in Amazon S3 bucket behind the scenes. 

You can later use the snapshot to create a new EBS volume for your EC2 instance so that no data is lost, especially when there is important data in the EBS volume.

---

## How to work with EBS Snapshot

First, you have to create a snapshot of the EBS volume.

This is going to capture the data at that moment.

Secondly, you have to save the snapshot, which AWS safely stores for you and can be used for backup and disaster recovery.

Thirdly, restore the snapshot when needed.

You can do this by using it to create a new EBS volume and then attaching it to your EC2 instance.

---

## Some benefits that come with EBS Snapshot

Some benefits that come with EBS snapshots are that they are incremental. What I mean is that when you take the first snapshot, it copies all the data, but the next snapshot only keeps the changes, not the entire data again.

## Let’s talk about Data Lifecycle Manager

This is the process of creating, managing, and deleting snapshots automatically.

Let’s look at it like this using a bank's record-keeping.

By law, banks have to keep customer records for 5 to 7 years. Imagine a bank with 8 million customers. Instead of a human manually trying to save every single statement, the Data Lifecycle Manager automatically takes a snapshot of the whole database where those records live.

It follows a 'retention rule it keeps that snapshot for exactly 7 years for compliance. But the second that time is up, it deletes it. Doing this manually for 8 million people would be a nightmare and full of mistakes but the Data lifecycle manager does it all in the background without you ever having to worry about it.

# Object Storage

### Let’s talk about Object Storage

Object storage is a cloud-based way to store a large amount of data, mostly unstructured data like videos, images, and so on.

All these objects come with an ID, attributes, and metadata to help you find and manage them. One important thing is that they are not stored in folders like the way we store files on our computer. Instead, they are stored together in a single storage space.

---

### Understanding Objects

Let me explain this very well.

An object is just a file we store on our system every day. It can be a media file, document, text file, or even programming files.

Each object comes with:

- **ID** – this is the unique identifier of the file  
- **Metadata** – this gives more details about the file like date created, size, etc.  
- **Attributes** – also gives extra information about the file  

---

### Types of Data

Objects can come in two forms:

**Structured Data**  
This is data arranged in rows and columns like a table (database).

**Unstructured Data**  
This is data that does not follow rows and columns like:

- Images  
- Videos  
- Text files  
- Social media posts  
- Sensor data  

Object storage is mainly designed for **unstructured data**.

---

## Amazon S3 (Simple Storage Service)

Now let’s move to Amazon S3 bucket, which is used for object storage.

Amazon S3 is an AWS service that allows you to store any amount of data using buckets.

It is:

- Scalable  
- Secure  
- Durable  

Your data is stored across different availability zones in a region for safety.

Each object stored in S3 comes with:

- Data  
- Key (this is like the file name/path)  
- ID  
- Metadata  

All your files are stored inside a bucket, and a bucket can hold a very large amount of data.

---

### What You Can Use S3 For

- Static website hosting  
- Application data storage  
- Backup  
- Content distribution  
- And more  

S3 also has something called **lifecycle**, which can automatically move your data between storage classes based on rules you set to save cost.

---

## S3 Storage Classes

Before we go into the types, let’s understand this.

S3 storage classes are different ways to store your data based on:

- How often you use it  
- Your budget  

---

### Types of S3 Storage Classes

**S3 Standard**  
Good for data you use regularly. Fast access and high availability, but more expensive.

---

**S3 Intelligent-Tiering**  
This automatically moves your data based on how often it is used to help you save money.

---

**S3 Standard-IA (Infrequent Access)**  
Used for data you don’t access often. Good for backup and cheaper than standard.

---

**S3 One Zone-IA**  
Cheaper because data is stored in only one availability zone. Not good for very important data.

---

**S3 Glacier Instant Retrieval**  
Low cost and still fast when you want to access your data.

---

**S3 Glacier Flexible Retrieval**  
Very cheap but slower to access. Good for backup and disaster recovery.

---

**S3 Glacier Deep Archive**  
The cheapest option. Good for data you rarely access, like long-term records (e.g., bank data).

More to be added soon.
