# ansible-homeserver

Very opinionated Ansible playbook to build out all my home server services. It has been tested against 64 bit Ubuntu on a Raspberry Pi 4.

It will install Certbot, CUPS, PiHole (Docker), Cloudflared(Docker), HomeAssistant (Docker), Homebridge (Docker), Zigbee2Mqtt (Docker) and and NGINX reverse proxy for TLS termination. Certbot will attempt to get a DNS01 challenged certificate using Cloudflare credentials in the all.yml vars file.

group_vars/all.yml needs to be created and the inventory file needs to be created to point at your server.

The user you run as will need sudo access to the server.

To do:
  - Option to run NGINX without certbot, IE BYO certififcates or self signed.

Run this at your own risk, be sure to understand everything it is doing before you let it loose in production or on your home network. You may very well have to modify it to your needs as it has been written for my specific use case as it stands.
