<img src="https://cdn.prod.website-files.com/677c400686e724409a5a7409/6790ad949cf622dc8dcd9fe4_nextwork-logo-leather.svg" alt="NextWork" width="300" />

# Connect a Web App with Aurora

**Project Link:** [View Project](http://learn.nextwork.org/projects/aws-databases-webapp)

**Author:** Lutendo Matshidze  
**Email:** lupreshie@gmail.com

---

## Connect a Web App to Amazon Aurora

![Image](http://learn.nextwork.org/charmed_beige_timid_seahorse/uploads/aws-databases-webapp_1709b26b)

---

## Introducing Today's Project!

### What is Amazon Aurora?

Amazon Aurora is a rational database and it is useful because it can hold large scale databases efficiently.

### How I used Amazon Aurora in this project

In today's project, I used Amazon Aurora to connect with a web app where I could add data  on the web app.

### One thing I didn't expect in this project was...

One thing I didn't expect in this project was how tangible databases are in being able to use data you've entered.

### This project took me...

This project took me 1 hour 30 minutes including the documentation.

---

## Creating a Web App

![Image](http://learn.nextwork.org/charmed_beige_timid_seahorse/uploads/aws-databases-webapp_b7999168)

To connect to my EC2 instance, I used the terminal to connect using `ssh -i NextWorkAuroraApp.pem ec2-user@ec2-13-247-224-44.af-south-1.compute.amazonaws.com` and I made sure that I had access to do so using the command `chmod 400`.

To help me create my web app, I first made sure that all my software on the EC2 instance was updated and that I installed all the tools (Apache, PHP, PHP-mysqli, MariaDB) I need on the EC2 to start the web app.

---

## Connecting my Web App to Aurora

I set up my EC2 instance's connection details to my database by using the terminal and by writing into the dbinfo.inc file using nano

![Image](http://learn.nextwork.org/charmed_beige_timid_seahorse/uploads/aws-databases-webapp_1709b25b)

---

## My Web App Upgrade

Next, I upgraded my web app by adding a SamplePage.php file that has a header and a form that I can add data info into.

![Image](http://learn.nextwork.org/charmed_beige_timid_seahorse/uploads/aws-databases-webapp_2709b25b)

---

## Testing my Web App

To make sure my web app was working correctly, I used MySQL CLI to ensure that I was able to retrieve all the data that I had entered through the web app.

![Image](http://learn.nextwork.org/charmed_beige_timid_seahorse/uploads/aws-databases-webapp_1409z22b)

---

---
