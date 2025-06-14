#   Nginx

## Modules Overview

###   Module 1: Introduction to Nginx
- **Topics**: What is Nginx?, Nginx  Use case
- **Demo**: Install Nginx (Ubuntu/rhel) and view the default welcome page

###   Module 2: Understanding Nginx Configuration
- **Topics**: nginx.conf, http/server/location blocks, directive syntax
- **Demo**: Modify config, change ports/logs, add custom error pages

###   Module 3: Hosting a Static Website
- **Topics**: Serving HTML, root directive, MIME types
- **Demo**: Replace welcome page with your custom static website

###   Module 4: Virtual Hosts (Server Blocks)
- **Topics**: server_name, root, multiple domains
- **Demo**: Set up two sites (e.g., `site1.local`, `site2.local`) using `/etc/hosts`

###   Module 5: Reverse Proxy Basics
- **Topics**: Reverse proxy, proxy_pass, headers
- **Demo**: Proxy requests to a Node.js or Flask app on another port

###   Module 6: Load Balancing
- **Topics**: Round-robin, health checks
- **Demo**: Balance traffic between two backends using Nginx

###   Module 7: SSL with Nginx (HTTPS)
- **Topics**: SSL/TLS basics, self-signed certs, Let's Encrypt
- **Demo**: Enable HTTPS using self-signed or Certbot certificates

###   Module 8: URL Rewrites and Redirects
- **Topics**: 301/302 redirects, rewrite, return
- **Demo**: Redirect `/old` to `/new`, force HTTPS redirection

###   Module 9: Nginx as a Caching Server
- **Topics**: Proxy cache, FastCGI cache, cache headers
- **Demo**: Enable caching, inspect `X-Cache-Status`

###   Module 10: Security and Hardening
- **Topics**: Path traversal prevention, method restriction, rate limiting
- **Demo**: Block IPs, allow internal-only access

###   Module 11: Monitoring and Logs
- **Topics**: Access/error logs, custom formats, tuning
- **Demo**: Analyze logs, define custom log format


### Module 1
- Nginx:
- It  is a high-performance web server that can also be used as a:
- Reverse proxy
- Load balancer
- HTTP cache
- Mail proxy

 ### Diff b/w  Traditional  Web Server & Event-Driven webserver:
 - new thread or process for each request
 - a small number of worker processes that can handle thousands of connections at the same time, using something called events.

 - Ex for Traditional
```bash
   One waiter per customer.
  100 customers = 100 waiters.
  Very busy, slow, and costly.
```
 - Ex for Event-driven
   
```bash
5  waiters with walkie-talkies.
They respond only when needed.
Handle 100+ customers without panic.
```
### Install and verify nginx on ubuntu and RHEL servers

```bash
sudo apt update
sudo apt install nginx -y
sudo systemctl start nginx
sudo systemctl enable nginx
systemctl status nginx
```
```bash
sudo yum install epel-release -y
sudo yum install nginx -y
sudo systemctl start nginx
sudo systemctl enable nginx
systemctl status nginx
```
- Open browser access nginx using http://<pub.ip>
- 










