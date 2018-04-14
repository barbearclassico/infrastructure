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


## Priority

- Setting up dropbox sync
- Load DB if is not set: download and build the latest from dropbox
- Load DB if is not set: install mysql
- Load DB if is not set: install users
- install 
- Put backup scripts in place
- install apache: get apache server
- install apache: download required modules
- install apache: get SSL barbearclassico - let's encrypt
- Setup mailgun
- Get SMF engine
- Get SMF theme
- Deploy newsletter phplist
- Deploy revive
- Deploy datadoghq
- Godaddy API
- firewall

