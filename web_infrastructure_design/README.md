# Web Infrastructure Design Project

This project aims to design scalable and secure web infrastructures, gradually building complexity. Each task involves whiteboarding and documentation to demonstrate an understanding of key components, their roles, and potential challenges.

## Learning Objectives

Upon completing this project, you should be able to:

- Draw a comprehensive diagram of the web stack built in sysadmin/devops track projects.
- Explain the functionalities of each component within the web stack.
- Describe the importance of system redundancy.
- Utilize acronyms such as LAMP, SPOF, QPS effectively.

## Tasks

### 0. Simple Web Stack

#### Requirements
- Design a one-server web infrastructure for www.foobar.com.
- Components: 1 server, 1 Nginx web server, 1 application server, 1 MySQL database, 1 code base.
- Configure domain name (foobar.com) with a www record pointing to server IP (8.8.8.8).
- Explain the roles of server, domain name, DNS record, web server, application server, and database.
- Identify issues: Single Point of Failure (SPOF), downtime during maintenance, scalability challenges.

**Files:**
- [0-simple_web_stack](0-simple_web_stack)


### 1. Distributed Web Infrastructure

#### Requirements
- Design a three-server web infrastructure for www.foobar.com.
- Add 2 servers, 1 HAproxy load balancer, 1 MySQL database.
- Explain reasons for additional elements.
- Describe load balancer's distribution algorithm and setup (Active-Active or Active-Passive).
- Explain Primary-Replica (Master-Slave) cluster in the database.
- Identify issues: Single Points of Failure (SPOF), security (no firewall, no HTTPS), lack of monitoring.

**Files:**
- [1-distributed_web_infrastructure](1-distributed_web_infrastructure)


### 2. Secured and Monitored Web Infrastructure

#### Requirements
- Design a three-server web infrastructure for www.foobar.com with security and monitoring.
- Add 3 firewalls, SSL certificate for HTTPS, and 3 monitoring clients.
- Explain the purpose of added elements.
- Discuss SSL termination at the load balancer, MySQL server issues, and server component uniformity problems.
- Identify issues: SSL termination, single MySQL server capable of accepting writes, uniform server components.

**Files:**
- [2-secured_and_monitored_web_infrastructure](2-secured_and_monitored_web_infrastructure)


### 3. Scale Up

#### Requirements
- Add one more server and configure HAproxy as a cluster with the existing one.
- Split components (web server, application server, database) with their own servers.
- Explain reasons for additional elements.

**Files:**
- [3-scale_up](3-scale_up)

