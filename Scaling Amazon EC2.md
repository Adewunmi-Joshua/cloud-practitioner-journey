# Scaling and Monitoring in AWS

Let’s dive into one of the most interesting parts of my learning journey.

**Scalability**, **Elasticity**, **Auto Scaling**, **Load Balancing**, and **CloudWatch**

First, I want you to look at all of them like **friends**, but each one has a different role to play.

## What Is Scalability?

Scalability is the ability of a system to grow and handle more workload without you worrying.

Scalability has two interesting parts:

- Vertical Scaling (Scaling Up)

- Horizontal Scaling (Scaling Out)

## What Is Vertical Scaling?

This is adding more power to the compute you already have, such as:

- More CPU

- More memory

- More storage 

Just imagine it like upgrading your system to a better and more powerful one.

## What Is Horizontal Scaling?

This is adding more compute resources to the ones you already have in order to handle traffic load.

Just imagine it like setting up different servers to help each other when there is large traffic, so one server will not be overwhelmed.

## Where CloudWatch and Load Balancing Come In

Now this is where **CloudWatch** and **Load Balancing** come in.

**CloudWatch** monitors the traffic going to each server.

If the traffic becomes too much on a particular server, it triggers an alert.

**Load Balancing** then directs traffic to other servers to prevent crashes and maintain the workload.

## Bank Analogy

Imagine you are in a bank with three cashiers ready to attend to customers:

The first cashier has about 30 people in the queue

The second cashier has about 5 people

The last cashier is just chilling because there is nobody to attend to

Now imagine someone is assigned to monitor this situation and make reports.
Look at that person as **CloudWatch**.

After the report is made, another person comes in to address the situation and directs people to the other cashiers to balance the workload and reduce stress on the cashier handling 30 people.
That is the work of **Load Balancing**.

## Elasticity

This is the process of **automatically** adjusting compute based on demand.
Let’s look at it this way: imagine you have an e-commerce website, but around December to April you always have huge traffic visiting your website. Elasticity makes it possible to add more compute to handle that huge traffic, and maybe around May to August when the traffic is low, it will reduce the compute back. This saves money because you only pay for what you use and need.

**Auto Scaling**: This is the implementation of elasticity. It is about adding more compute when needed and reducing compute when it is not needed automatically, and Auto Scaling can only happen when it is added to your application.
