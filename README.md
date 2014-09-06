Config
======

This repository contains the configuration information necessary to host our applications in high availability, optimally performing production enviornments.

All of our servers run on RHEL 6/7.

Node / Meteor.js
----------------

The node production stack uses NGINX, systemd.service, node processes, and MongoDB.

- NGINX serves as a reverse proxy SSL server and load balancer.
- systemd.service ensures all critical processes stay running or restart in the case they stop.
- Multiple node processes are hosted for performance increases.
- MongoDB is used for data persistence.
