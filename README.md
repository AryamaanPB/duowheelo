# DuoWheelo
#### Aryamaan Singh

This is my attempt at trying to get my hands dirty with Django Rest Framework while working with PostgreSQL, RabbitMQ, Docker etc to build APIs for an online bike store.

## Aim
Here I am listing a few of the features that I hope to incorporate in this project:
- APIs that can allow the users, to log in and signup
- APIs that can let him and his staff members update the inventory
- APIs with which users can purchase a bike, Both ONLINE and OFFLINE payment modes are available.
- APIs to handle order cancellation and refund
- APIs where the users can see their previously ordered bikes and how much warranty is left.
- APIs that can book a servicing appointment for a user
- Once an appointment has been booked someone from John’s team would eventually assign a technician to handle the bike servicing.
- The same person would also add an expected time by which the bike servicing will be completed.
- APIs to handle the payment for booking a servicing appointment, Both Online and Offline payment     modes are available. (Bypass Payment Gateway)
- A python script that can generate invoices for the orders that will be created by
the application. This script will be continuously listening for messages coming to a RabbitMQ/Redis queue. As soon as a message is pushed to the queue, this script will pull the message, extract the essential user details from the message, and then create a PDF out of that data, and store the file somewhere in the filesystem.