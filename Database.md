## Database  ( AWS )

Let talk about database, which is one of the interesting topics under my AWS learning journey.  

But what is a database? Let look at it like this for clarity:  

Imagine someone called henry comes back home with a lot of gifts at hand from a supermarket he has been buying from since 2017. But something interesting is that when he was explaining himself to his friend, he said not everyone has access to the gifts because the company only gives them to customers with a consistent long record.  

But wait, how did the company know that?  

Thanks to a database. It is where all the customer information is stored, made up of tables with rows and columns.  

I will discuss more about this in the coming documentation, from how AWS shared responsibility is attached to the databases AWS has to offer.

## Let move a little bit forward  

Let move a little bit forward by talking about two types of database: relational database and non-relational database.

---

### What is relational database?  

This is the process of storing data using rows and columns, and each table in the database can be linked to each other based on the relationship of the data, using SQL.

Let me make this clear very well. Remember the example I used at the beginning of this chapter about someone buying things from a particular supermarket for years.  

For the store to decide if it is worth giving gifts, they are going to check purchase records, transaction records, and other related data. The reason they do this is because all the data is related to each other.  

So, same as a relational database, it is a set of data that is linked together.

---

### What is non-relational database?  

This is the process of storing data in a flexible way without using rows and columns, like documents, graphs, and so on.  

It is good for data that changes frequently and also good if you are looking for something with high performance and scalability with no fixed structure. It makes use of NoSQL.

---

### Let make it more clear  

Imagine you have a store in your house. You will agree with me that there is no strict rule on what you can drop there—shovel, cutlass, bag, and other materials can be stored there in any way.  

Same as a non-relational database, it is flexible and different formats of data can be stored.  

But a relational database must be well structured and arranged in a way that the data corresponds with each other.

## Let talk about AWS Relational Database (Amazon RDS)

Let talk about AWS relational database, which is one of their services called Amazon RDS.

It is used for managing relational databases with a fully managed process like setup, patching, backups, and maintenance, so you can focus on other things you need to do.

Not only that, it is very reliable because it supports multi-AZ (multiple availability zone) deployment. This means that if one zone fails, it can fail over to another zone and keep operating.
 
It also comes with strong security features like VPC integration and data encryption.

### What is Amazon Aurora ? 

Another good thing is that you only pay for what you use, which helps reduce cost and stress.

Amazon RDS also supports different database engines like MySQL, Oracle, Microsoft SQL Server, and others.
