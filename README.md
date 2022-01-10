# ansible-homeserver

Ansible playbook to build out all my home server services. It has been tested against Ubuntu 64Bit on a Raspberry Pi 4.

It will install Certbot, CUPS, PiHole (Docker), Cloudflared(Docker), HomeAssistant (Docker), Homebridge (Docker), Zigbee2Mqtt (Docker) and and NGINX reverse proxy. Certbot will attempt to get a DNS01 challenged certificate using credentials in the all.yml vars file.

all.yml needs to be modified and the inventory file needs creating to point at your server.

The user you run as will need sudo access to the server.

To do:
  - Modules
  - General tidying