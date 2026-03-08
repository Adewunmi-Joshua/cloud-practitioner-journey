# Storage

In this section I will be discussing what cloud storage is, types of cloud storage, Amazon S3, S3 storage classes and so on.

So let get started.


## What is Cloud Storage

This is a kind of service that allows users to access data, manage data, and save data over the internet instead of them having a physical storage hard drive themselves, which is going to cost a lot and require maintenance. 

Another interesting thing is that you are only going to pay for what you use, which is one reason big organisations love to use it.

---

## Type of Storage

### Block Storage

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

More to be added soon.
