# AWS Security

Let dive into how to protect data in the AWS Cloud, and one aspect I want to focus on especially is IAM (Identity and Access Management) section as career. As they always say, to use a product, it must be secure. Same as AWS Cloud, this section is very important and is not taken lightly at all, so a lot of things are put in place to protect people data in the cloud.

So let start looking into it.

## Data Encryption

What is that? It is like you have heard about encryption before, yes you have, you just don’t know we use it in our daily activities.

To make it easy, let look at it like this:

Imagine a particular house door is locked and the house owner is not around, but is telling you to have access to the house. Without the key, or if the person did not hand you the right key, you will agree with me that you will not be able to enter the house until you have the right key.

Encryption works like a key mechanism also, where you must have the right key to unlock or have access to particular data.

Encryption is also used to turn customer data into unreadable characters that people will not understand, especially hackers.

Imagine someone’s name is Henry, and it appears like unreadable information when encrypted. Without the right key, it will be difficult for someone to understand the real information.

## Type of Encryption

Firstly, we have **Encryption at Rest**: what this actually means is that the data is being stored and is not currently in use or processing.

Secondly, we have **Encryption in Transit**: this is the opposite here, where the data is being used and processed.

A good example is when you request for your Skill Builder password and it is sent from the server to your application. Just put this in mind: it is moving data.

---

## Let talk about AWS Data Protection

### AWS Key Management Service (KMS)

This is used to create, store, and manage cryptographic keys, which are used to encrypt and decrypt data, and it can be used across multiple AWS services in your application.

---

### Cloud Hardware Security Module (CloudHSM)

This allows you to securely store and manage cryptographic keys in dedicated hardware in the cloud.

It acts like a private safe place in the cloud where you can trust highly sensitive keys with strong security protection.

Another interesting thing is that you don’t have to stress yourself owning or maintaining this kind of expensive hardware when you can host it with AWS Cloud or another cloud provider.

Let just imagine it like this: I don’t know if you have stored your data, especially MFA passkeys, in a USB hardware device before, where it asks you to plug it into your system before having access to a website or whatever you are using it for.

Now imagine that kind of USB hardware hosted in the cloud with stronger protection than taking care of it yourself.

More is coming

