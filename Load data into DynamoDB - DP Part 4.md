<img src="https://cdn.prod.website-files.com/677c400686e724409a5a7409/6790ad949cf622dc8dcd9fe4_nextwork-logo-leather.svg" alt="NextWork" width="300" />

# Load Data into DynamoDB

**Project Link:** [View Project](http://learn.nextwork.org/projects/aws-databases-dynamodb)

**Author:** Lutendo Matshidze  
**Email:** lupreshie@gmail.com

---

## Load Data into a DynamoDB Table

![Image](http://learn.nextwork.org/charmed_beige_timid_seahorse/uploads/aws-databases-dynamodb_b481c730)

---

## Introducing Today's Project!

### What is Amazon DynamoDB?

Amazon DynamoDB is a non-relational database service that organizes data using key-pairs.

### How I used Amazon DynamoDB in this project

In today's project, I used Amazon DynamoDB to create five tables. I ised Cloushell and CLI to load data into my tables quickly. I also compared DynamoDB to relational database by understanding how items anf attributes work!

### One thing I didn't expect in this project was...

One thing I didn't expect in this project is that I can performa lot of actions using AWS CLI instead of the console e.g creating and deletign tables, loading data etc..

### This project took me...

This project took me 60 minutes including documentation and understanding time.

---

## Create a DynamoDB table

DynamoDB tables organize data using items and attributes. Every single item is recorded with a set of attributes. Item can have any number of attriubutes with a minimum 1 for the partition key.

An attribute is a piece of data about an item in the DynamoDB table. For example , if the item was a specific NextWork student, attributes could be StudentName, ProjectsComplete, Email, SignUpDate....the number of attributes for each item is flexible.

![Image](http://learn.nextwork.org/charmed_beige_timid_seahorse/uploads/aws-databases-dynamodb_a3cefee0)

---

## Read and Write Capacity

Read capacity units (RCUs) and write capacity units (WCUs) are units that measure my DynamoDB tables performance. DynamoDB pricing is based on RCUs and WCUs. So the more RCUs and WCUs consumed the more ecpensive the project.

Amazon DynamoDB's Free Tier covers 25 RCUs and WCUs monthly. I turned off auto scaling because this can result in higher charges of DynamoDB automatically scales up my operations which charges more RCUs and WCUs.

![Image](http://learn.nextwork.org/charmed_beige_timid_seahorse/uploads/aws-databases-dynamodb_ef47dd8f)

---

## Using CLI and CloudShell

AWS CloudShell is an enviroment that lets us run code to interact with our AWS resources/services. Using AWS Cloudshell is handy because AWS CLI is pre-installed so we can run commands right away.

AWS CLI is a software that lets you interact with resources using commands instead of clicks in the console. This is a very practical softeware that is prefered over using the AWS Management Console in day to day engineering operations in the real world.

I ran a CLI command in AWS CloudShell that created foour new DynamoDB tables. The AWS CLI command is called `aws dynamodb create-table`, and could define the table name and its attributes all within the command.

![Image](http://learn.nextwork.org/charmed_beige_timid_seahorse/uploads/aws-databases-dynamodb_81e0258b)

---

## Loading Data with CLI

I ran a CLI command in AWS CloudShell that load mulriple pieces of data i.e load multiple items)  DynamoDB tables set up in the previous step. This AWS is structurd as `aws dynamodb batch-write-item --request-items file://x`.

![Image](http://learn.nextwork.org/charmed_beige_timid_seahorse/uploads/aws-databases-dynamodb_791c600b)

---

## Observing Item Attributes

![Image](http://learn.nextwork.org/charmed_beige_timid_seahorse/uploads/aws-databases-dynamodb_b481c731)

I checked a ContentCatalog item, which had the following attributes: ContentType, Price, Services, Title, UR etc..

I checked another ContentCatalog item, which had a different set of attributes: Services, Title, VideoType etc..

---

## Benefits of DynamoDB

A benefit of DynamoDB over rational databases is flexibilty, because items can have their own set of attributes. This is great for scenarios where a table has different kinds of data and some attributes don't apply to all data in that table.

Another benefit over relational databases is speed, because DynamoDB can partition its data to narrow down the search using partition keys. This is faster than relational databases which need to scan the entire table to find pieces of data.

![Image](http://learn.nextwork.org/charmed_beige_timid_seahorse/uploads/aws-databases-dynamodb_b481c730)

---

---
