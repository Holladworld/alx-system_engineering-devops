# 0x09. Web infrastructure design

[![Webinfrastucture image](https://miro.medium.com/v2/resize:fit:1034/1*xKd1CchSaSKV83Oizju8kg.png)]

## Resources:books:
Read or watch:
* [Network basics](https://intranet.hbtn.io/rltoken/Sn9ZSSHjyEW5aRfKvNiZCg)
* [Server](https://intranet.hbtn.io/rltoken/83joH7-HzuV9gBNe16iTrA)
* [Web server](https://intranet.hbtn.io/rltoken/7moqhXcFOXP6zNMWdsjWjQ)
* [DNS](https://intranet.hbtn.io/rltoken/G0a1v98rwb2RHA8VHxo36A)
* [Load balancer](https://intranet.hbtn.io/rltoken/H6TVgGaqt13JhXKzJ2rVAA)
* [Monitoring](https://intranet.hbtn.io/rltoken/JY6524JCvX9dREoNgnQUFw)
* [What is a database](https://intranet.hbtn.io/rltoken/XLIOfzfuaxPQu39VQ0TLtw)
* [What’s the difference between a web server and an app server?](https://intranet.hbtn.io/rltoken/Nb8B47Y2D8SLqQMOKVoQyQ)
* [DNS record types](https://intranet.hbtn.io/rltoken/pSGVxlKznxONwGEHIXLSwA)
* [Single point of failure](https://intranet.hbtn.io/rltoken/wYpewVpIp9PSqqL27RPafg)
* [How to avoid downtime when deploying new code](https://intranet.hbtn.io/rltoken/Mlvynt0OgLQXrxjrC5Wlnw)
* [High availability cluster (active-active/active-passive)](https://intranet.hbtn.io/rltoken/POX3jE0S6TChQHSYQraYeQ)
* [What is HTTPS](https://intranet.hbtn.io/rltoken/N4BwU4wYDNW02kdzMiekFw)
* [What is a firewall](https://intranet.hbtn.io/rltoken/HrYI70d_nxUPZeufjUYzIw)

---
## Learning Objectives:bulb:
What you should learn from this project:

* You must be able to draw a diagram covering the web stack you built with the sysadmin/devops track projects
* You must be able to explain what each component is doing
* You must be able to explain system redundancy
* Know all the mentioned acronyms: LAMP, SPOF, QPS

---

### [0. Simple web stack](./0-simple_web_stack)
On a whiteboard, design a one server web infrastructure that hosts the website that is reachable via www.foobar.com. Start your explanation by having a user wanting to access your website.
You must use:
* 1 physical server
* 1 web server (Nginx)
* 1 application server
* 1 application files (your code base)
* 1 database (MySQL)
* 1 domain name foobar.com configured with a www record that points to your server IP 8.8.8.8


### [1. Distributed web infrastructure](./1-distributed_web_infrastructure)
On a whiteboard, design a three servers web infrastructure that host the website www.foobar.com.
You must add to 0-simple_web_stack:
* 2 physical servers
* 1 web server (Nginx)
* 1 application server
* 1 load-balancer (HAproxy)
* 1 application files (your code base)
* 1 database (MySQL)


### [2. Secured and monitored web infrastructure](./2-secured_and_monitored_web_infrastructure)
On a whiteboard, design a three servers web infrastructure that host the website www.foobar.com, it must be secured, serve encrypted traffic and be monitored.
You must add to 1-distributed_web_infrastructure:
* 3 firewalls
* 1 SSL certificate to serve www.foobar.com over HTTPS
* 3 monitoring clients (data collector for Sumologic or other monitoring services)

### [3. Scale up](./3-scale_up)
You must add to 2-secured_and_monitored_web_infrastructure:
* 1 physical server
* 1 load-balancer (HAproxy) configured as cluster with the other one
* Split components (web server, application server, database) with their own server
