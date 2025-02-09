# 🏠 Homelab Project
This repository is a WIP to learn more about self-hosting, kubernetes, and creating a secure homelab. 

## 🖥️ Hardware
### Current Setup
- [Beelink EQ14 Mini PC](https://www.amazon.co.uk/dp/B09XGZ3RTM) x 2 - Compact but powerful mini PCs with AMD Ryzen 7 5800H, 32GB RAM, and 500GB SSD

### Coming Soon
- [Tecmojo 9U Wall Mount Rack](https://www.amazon.co.uk/gp/product/B0DBRBKRS6) - Professional 9U network cabinet for organizing network equipment and servers
- [UniFi Dream Machine Pro](https://uk.store.ui.com/uk/en/products/udm-pro) - Enterprise-grade router/firewall with built-in Network Controller, 10G ports, and advanced security features (IPS/IDS)

## 🛠️ Infrastructure
### Core Software
- [Proxmox](https://www.proxmox.com/en/) - Enterprise-class hypervisor for running and managing multiple virtual machines and containers
- [Ubuntu 24.04.1 LTS](https://ubuntu.com/download/server) - Latest LTS release of Ubuntu Server, providing a stable and secure base OS with 5 years of support

### Kubernetes Stack
- [k3s](https://k3s.io/) - Lightweight Kubernetes distribution perfect for edge, IoT, and homelab environments (uses just 512MB RAM)
- [FluxCD](https://fluxcd.io/) - GitOps toolkit for automating Kubernetes deployments using a Git repository as the source of truth
- [Kustomize](https://kustomize.io/) - Template-free way to customize Kubernetes manifests for different environments
- [Aaptakube](https://aptakube.com/) - Modern, native macOS GUI for managing Kubernetes clusters with a clean interface

## 🚀 Apps Running
### Infrastructure & Security
- [Cloudflare Tunnel](https://developers.cloudflare.com/cloudflare-one/connections/connect-networks/) - Secure, zero-trust tunnel to expose services without opening ports or managing DNS

### Monitoring
- [Grafana](https://grafana.com/) - Feature-rich platform for metrics visualization, alerting, and dashboards
- [Prometheus](https://prometheus.io/) - Time-series database and monitoring system with powerful querying and alerting capabilities

### Applications
- [Ghost](https://ghost.org/) - Modern, open-source publishing platform with a clean interface and membership capabilities
- [Home Assistant](https://www.home-assistant.io/) - Open source home automation platform that puts local control and privacy first
- [Hoarder](https://hoarder.app/) - AI-powered bookmarking tool that automatically tags and organizes saved content
- [IT Tools](https://github.com/CorentinTh/it-tools) - Collection of utilities for developers including encoders, formatters, and generators

### Databases
- [PGVector](https://github.com/pgvector/pgvector) - PostgreSQL extension for vector similarity search, enabling AI and ML applications

## 📚 Resources
- [Fantastic tutorial on setting up a homelab](https://bash.ghost.io/) - Comprehensive guide covering hardware selection to software deployment
- [Securely expose your homelab using Cloudflare](https://github.com/adyanth/cloudflare-operator) - Tutorial on implementing zero-trust access with Cloudflare
- [GitOps with ArgoCD](https://confixa.medium.com/a-step-by-step-guide-of-kubernetes-deployment-with-argo-cd-for-nodejs-application-31746a41a5d1) - Step-by-step guide for implementing GitOps workflows
- [k3s Cluser with Ansible](https://axivo.com/k3s-cluster/) - Automated k3s cluster setup using Ansible playbooks

## 🎯 Tech Learning Roadmap

### Infrastructure & OS
- [Talos OS](https://www.talos.dev/) - Security-focused, minimal Linux OS designed specifically for running Kubernetes, with immutable infrastructure
- [Amazon EKS via eksctl](https://eksctl.io/) - Official CLI tool for Amazon EKS that simplifies cluster creation and management

### Infrastructure as Code
- [Pulumi](https://www.pulumi.com/) - Modern IaC platform using familiar programming languages (TypeScript, Python, Go) instead of DSLs
- [OpenTofu](https://opentofu.org/) - Community-driven, open source fork of Terraform maintaining compatibility while ensuring long-term sustainability

### Container Management
- [Portainer](https://www.portainer.io/) - Lightweight container management UI with support for Docker, Kubernetes, and edge environments
- [Docker Stack](https://www.youtube.com/watch?v=ZmL46xVdYzM) - Advanced Docker Compose feature for managing multi-container applications in swarm mode
- [ArgoCD](https://argo-cd.readthedocs.io/en/stable/) - Declarative GitOps tool for Kubernetes with a rich UI and automated sync capabilities

### Networking & Proxy
- [Caddy](https://caddyserver.com/) - Modern web server with automatic HTTPS, HTTP/3 support, and simple configuration syntax
- [Traefik](https://traefik.io/traefik/) - Cloud-native edge router that auto-discovers services and handles SSL termination

### Monitoring & Management
- [RenovateBot](https://docs.renovatebot.com/) - Automated dependency updates across multiple package ecosystems with fine-grained controls
- [UptimeRobot](https://uptimerobot.com/) - Website monitoring service that checks your sites every 5 minutes and alerts on downtime 