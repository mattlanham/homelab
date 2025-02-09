# 🏠 Homelab Project
This repository is a WIP to learn more about self-hosting, kubernetes, and creating a secure homelab. 

## 🖥️ Hardware
### Current Setup
- [Beelink EQ14 Mini PC](https://www.amazon.co.uk/dp/B09XGZ3RTM) x 2

### Coming Soon
- [Tecmojo 9U Wall Mount Rack](https://www.amazon.co.uk/gp/product/B0DBRBKRS6) - Rack for other hardware
- [UniFi Dream Machine Pro](https://uk.store.ui.com/uk/en/products/udm-pro) - 10G Cloud Gateway with IPS/IDS and UniFi OS

## 🛠️ Infrastructure
### Core Software
- [Proxmox](https://www.proxmox.com/en/) - manages the VMs
- [Ubuntu 24.04.1 LTS](https://ubuntu.com/download/server) - OS

### Kubernetes Stack
- [k3s](https://k3s.io/) - Lightweight k8s
- [FluxCD](https://fluxcd.io/) - GitOps
- [Kustomize](https://kustomize.io/) - Native k8s config manager
- [Aaptakube](https://aptakube.com/) - k8s GUI for Mac

## 🚀 Apps Running
### Infrastructure & Security
- [Cloudflare Tunnel](https://developers.cloudflare.com/cloudflare-one/connections/connect-networks/) - Connect to the homelab from the internet (securely)

### Monitoring
- [Grafana](https://grafana.com/) - Monitoring
- [Prometheus](https://prometheus.io/) - Monitoring

### Applications
- [Ghost](https://ghost.org/) - Blog software
- [Hoarder](https://hoarder.app/) - Bookmarking+ (ai tags, easy to use)
- [IT Tools](https://github.com/CorentinTh/it-tools) - Collection of handy online tools for developers

### Databases
- [PGVector](https://github.com/pgvector/pgvector) - Open-source vector similarity search for PostgreSQL

## 📚 Resources
- [Fantastic tutorial on setting up a homelab](https://bash.ghost.io/)
- [Securely expose your homelab using Cloudflare](https://github.com/adyanth/cloudflare-operator)
- [GitOps with ArgoCD](https://confixa.medium.com/a-step-by-step-guide-of-kubernetes-deployment-with-argo-cd-for-nodejs-application-31746a41a5d1)
- [k3s Cluser with Ansible](https://axivo.com/k3s-cluster/)

## 🎯 Tech Learning Roadmap

### Infrastructure & OS
- [Talos OS](https://www.talos.dev/) - Linux OS specifically for k8s
- [Amazon EKS via eksctl](https://eksctl.io/) - Makes managing k8s on AWS easier

### Infrastructure as Code
- [Pulumi](https://www.pulumi.com/) - Infrastructure as code including js/ts
- [OpenTofu](https://opentofu.org/) - Open source fork of Terraform for infrastructure as code

### Container Management
- [Portainer](https://www.portainer.io/) - Docker container management
- [Docker Stack](https://www.youtube.com/watch?v=ZmL46xVdYzM) - Docker Compose in swarm mode for container orchestration
- [ArgoCD](https://argo-cd.readthedocs.io/en/stable/) - Alternative GitOps tool to compare with FluxCD

### Networking & Proxy
- [Caddy](https://caddyserver.com/) - Modern, automatic HTTPS web server
- [Traefik](https://traefik.io/traefik/) - Cloud native application proxy and load balancer

### Monitoring & Management
- [RenovateBot](https://docs.renovatebot.com/) - Auto update versions (docker images)
- [UptimeRobot](https://uptimerobot.com/) - Uptime Monitor 