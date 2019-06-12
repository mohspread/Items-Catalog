# Udacity Linux / Ubuntu server project for Full Stack course
This is related to the catalog local server project, completed earlier in the course.
The aim is to host the catalog app on Amazon's AWS Lightsail virtual private server project, configure the code AND change the database storing the information to a Postgresql database.

The code for the origional catalog app project can be seen on my github [here](https://github.com/dcfwight/catalog.git)

Created by Doug Wight - dcfwight@gmail.com

## IP Address of server:
[http://34.241.100.161](http://34.241.100.161)

## Summary of software installed
Apache webserver using Flask framework and bootstrap formatting.  
Data is saved to a Postgresql database on the server.

## Configurations made
1. Root access disabled
1. Postgresql user called 'catalog' added, with password 'REDACTED'
1. An additional superuser called 'grader' was added to allow Udacity grader to access the server. This user has since been **REMOVED**
1. Password access to the server disabled
1. Access limited to private rsa key authentication
1. Enabled firewall to restrict ports to 2200 for ssh, 80 for webservice, 123 for NTP. All others ports have been blocked.
1. The ssh port is 2200 - a non-default port. The normal port (22) has been disabled.

## Login instructions
1. Access the server by using the private rsa key provided
1. E.g. enter the following command in a terminal to gain access to the ubuntu server:


`ssh ubuntu@34.21.100.161 -p 2200 -i ~PATH-TO-SAVED-PRIVATE-RSA-KEY`


## Third party resources used
Many!!! Particularly Udacity forum posts and links from there.
Some of these included:

[Programming knowledge youtube link on configuring Postgresql](https://www.youtube.com/watch?v=-LwI4HMR_Eg)


[Digital Ocean set-up tutorial on apache and python for ubuntu](https://www.digitalocean.com/community/tutorials/how-to-set-up-an-apache-mysql-and-python-lamp-server-without-frameworks-on-ubuntu-14-04)
