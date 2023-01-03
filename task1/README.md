
## Main goal:
Automate entirely provision and deploy wordpress website on pure bare metal server so the final result should have been a Welcome page to installation process when typing it's address in browser. So basically, once a playbook is done there should be just one command which is deploying and provisioning everything in order to have the final browser's response - a Welcome page.



## Task prescriptions and requirements:
- You will have to write ansible playbook which will manage each task for provisioning.
- You will have to have at least 2 VMs, one is controller node and a slave one which will be managed by host.
- All the services, applications required for Wordpress functioning should be deployed within the Docker container(s), it doesn't matter with docker cli engine or docker-compose, swarm etc.
- Wordpress archive content shouldn't be uploaded on host machine
- Wordpress stack - nginx+php-fpm+mysql
- Slave should be absolutely bare, everything which is requiring some dependencies should be provisioned and mentioned in playbook

## Allowed:

> To preconfigure passwordless ssh access onto slave node from master node before launching a playbook
> 
> To use OSs on your own, on both master and slave
> 
> To prepare configuration files for webserver, dbserver, php-fpm etc. before starting deploy/provisioning
> 
> HTTP or HTTPS is not mandatory
> 
> The less warnings you will be getting during the provision the more awards you will be achieving :)
> 
> Do try using native ansible modules rather than command or shell modules

