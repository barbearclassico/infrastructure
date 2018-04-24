# Infrastructure

This project is to deploy the whole Barbearclassico websitethrough ansible playbooks.

This is a work in progress.


## Design

Services in use:

* OVH
* godaddy
* Mailgun
* Dropbox
* Datadoghq
* SMF


## Build

Execute the command to deploy a VM

    vagrant up

Provision the instance:

    vagrant provision


## Priority


### DONE:

- Setting up dropbox sync /opt/bctools/

### TODO:

- Put backup scripts in place /opt/bctools/

- MySQL 
    - install mysql
    - create users
    - download and build the latest backup from dropbox
    
- NGINX
   - get nginx server 
   - install nginx: download required modules
   - configure maxmind geolocation
   - get SSL barbearclassico - let's encrypt

- Forum: 
    - Get SMF engine /srv/bc/forum
    - Get SMF theme  /srv/bc/forum

- Forum Tools:
    - BCTelegram     /opt/bctools/
    - photoselector  /srv/bc/photoselector
    - Deploy newsletter phplist /srv/bc/phplist
    - Deploy revive           /srv/bc/revive

- Core:
    - MAIL (Setup mailgun)
    - Deploy datadoghq
    - Godaddy API   /opt/bctools/bcgodaddy
    - firewall

