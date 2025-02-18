# ansible_provision-sonic

This Playbook will configure the necessary services(DHCP, HTTPD, ZTP) on a server for the purposes of PXEbooting SONiC compatible switches and then configuring them via Zero-Touch Provisioning.

The config_db.json is configured from a custom sonic-broadcom image I built for 100GbE Celestica switches so some tweaks might need to be made.

The configurations included will configure switches in a spine/leaf architecture if the switches are interconnected on the correct ports. MC-LAG will need to be configured manually if needed.

## Instructions
Download sonic-broadcom.bin from https://sonic.software/ or build your own.

Add sonic-broadcom.bin to ./roles/configs/files/ 

Edit variables in ./group_vars/all.yml

Run playbook
