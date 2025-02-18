# ansible_provision-sonic

This Playbook will configure the necessary services(DHCP, HTTPD, ZTP) on a server for the purposes of PXEbooting SONiC switches and then configuring them via Zero-Touch Provisioning.

## Instructions
Download sonic-broadcom.bin from https://sonic.software/ or build your own.

Add sonic-broadcom.bin to ./roles/configs/files/ 

Edit variables in ./group_vars/all.yml

Run playbook
