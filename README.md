#   Nginx
---

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




