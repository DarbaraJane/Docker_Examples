# Docker_New

## A brief summary
We will have two docker hosts currently existing in parallel, Charlie and Vaggie, with containers being managed with Docker Compose commands. As of 4/23/26 only one has been configured. Currently, the compose files exist at /opt/docker/



## Host 1
This exists on the proxmox host adminnode.

- IP Address: <Address>
- Memory: 11.72 GB
- Processors 4 (2 sockets, 2 cores)
- Storage: 192G
- Network: Bridge=vmbr0

### Containers
- checkmk
- cloudflare
- tools
- traefik

- uptimekuma
    - downtime alerts
- vaultwarden
    - password manager
- whoami
    - exists for testing.
- zammad-docker-compose
    - Legacy from demo for potential ticketing solution

## Host 2- Vaggie
To be installed on Second host

### Containerss
- cloudflare
- traefik
- DockGE or Komodo

## FAQs
- Why two hosts?
- Why do they both have cloudflare and traefik?
