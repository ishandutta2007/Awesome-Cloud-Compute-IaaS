<p align="center">
  <img src="assets/banner.svg" alt="Awesome Cloud Compute IaaS Banner" width="100%">
</p>

# ⚡ Awesome Cloud Compute IaaS (Infrastructure-as-a-Service)

<p align="center">
  <a href="https://github.com/ishandutta2007/Awesome-Awesome-Awesome"><img src="https://img.shields.io/badge/Awesome-%E2%9C%94-blueviolet?style=flat-square&logo=github" alt="Awesome"/></a>
  <a href="https://discord.gg/jc4xtF58Ve"><img src="https://img.shields.io/badge/Discord-5865F2?style=for-the-badge&logo=discord&logoColor=white" alt="Discord" /></a>
  <img src="https://img.shields.io/badge/License-Apache_2.0-blue.svg" alt="License" />
  <img src="https://img.shields.io/badge/Maintained%3F-yes-green.svg" alt="Maintained" />
  <a href="https://github.com/ishandutta2007"><img alt="GitHub followers" src="https://img.shields.io/github/followers/ishandutta2007?label=Follow" /></a>
</p>

> **A curated directory of top Cloud Compute (IaaS) SaaS providers, hypervisors, and open-source cloud virtualization platforms.**
> 
> *Explore virtual machines, bare metal servers, GPU instances, and infrastructure orchestration engines.*

---

## 📖 Table of Contents
- [🌐 Overview & Market Context](#-overview--market-context)
- [☁️ SaaS / Hosted IaaS Platforms](#️-saas--hosted-iaas-platforms)
- [🔓 Open-Source GitHub Projects](#-open-source-github-projects)
- [🤝 How to Contribute](#-how-to-contribute)
- [💖 Support & Sponsorship](#-support--sponsorship)
- [⭐ Star History](#-star-history)
- [⚠️ Disclaimer](#-disclaimer)

---

## 🌐 Overview & Market Context

This repository tracks notable **SaaS platforms** and **open-source projects** for **Cloud Compute (Infrastructure-as-a-Service / IaaS)**. Cloud compute tools enable developers, DevOps engineers, and cloud architects to provision virtual machines, bare metal infrastructure, GPU instances, and container runtime environments on-demand.

### 📊 Market Size & Industry Dynamics
> **Market Size & Structure**: The global Infrastructure-as-a-Service (IaaS) market is estimated at **~$180 Billion in 2026** and projected to surpass **~$500 Billion by 2032** (~19% CAGR). The sector is **highly concentrated at the top tier**, where hyperscalers (AWS, Microsoft Azure, and Google Cloud) capture **~63% of total global spending**. Meanwhile, a vibrant second tier of specialized independent clouds (DigitalOcean, Linode/Akamai, Vultr, Hetzner, OVHcloud) competes on developer experience, transparent pricing, and regional sovereignty.

---

## ☁️ SaaS / Hosted IaaS Platforms

Below is a curated table of leading proprietary and hosted cloud compute providers sorted by **Company Size / Annual Revenue** (descending).

| Platform | Description | Pricing (Starting Tier) | Free Tier / Trial Limits | Company Size / Revenue (Descending) |
| :--- | :--- | :--- | :--- | :--- |
| **[Amazon EC2](https://aws.amazon.com/ec2/)** | The industry-standard hyperscaler IaaS. Offers 700+ instance types, global availability zones, custom Graviton CPUs, and deep ecosystem integration. | **T4g.nano** (2 vCPU, 0.5 GiB): **~$0.0042/hour** (~$3.00/month). **M6g.medium** (1 vCPU, 4 GiB): **~$0.0385/hour** (~$28/month). Up to 60% savings on 3-yr reserved instances. | **750 hours/month** of `t2.micro` or `t3.micro` for **12 months** (new accounts). Always Free tier includes 750 hours/month in select regions. | **~$638 Billion** (Amazon FY2025 Revenue) |
| **[Google Compute Engine](https://cloud.google.com/products/compute)** | Google Cloud's IaaS platform featuring custom machine types, sustained-use discounts, live migration, and seamless GKE integration. | **e2-micro** (0.25 vCPU, 1 GiB): **~$0.0084/hour** (~$6.11/month). **e2-small** (0.5 vCPU, 2 GiB): **~$0.0168/hour** (~$12.23/month). | **$300 credit for 90 days** (free trial). Always Free: **1 `e2-micro` instance/month** (US regions) + 30 GB storage. | **~$350 Billion** (Alphabet FY2025 Revenue) |
| **[Microsoft Azure VMs](https://azure.microsoft.com/en-us/products/virtual-machines/)** | Enterprise-grade IaaS with 700+ VM sizes, strong hybrid cloud management via Azure Arc, and active directory integration. | **B1s** (1 vCPU, 1 GiB): **~$0.0104/hour** (~$7.59/month). **D2ads_v5** (2 vCPU, 8 GiB): **~$0.18/hour** (~$135/month). | **$200 credit for 30 days** + **750 hours of `B1s` Linux/Windows** for **12 months**. | **~$281 Billion** (Microsoft FY2025 Revenue) |
| **[Alibaba Cloud ECS](https://www.alibabacloud.com/product/ecs)** | Leading Cloud IaaS in Asia-Pacific with comprehensive global footprint, preemptible instances, and high-density compute nodes. | **ecs.u1-c1m2.large** (2 vCPU, 4 GiB): **~$0.05/hour** (~$36/month). Preemptible instances up to 90% discount. | **Free Trial Package**: Up to **12 months free trial** on select compute resources for verified new accounts. | **~$130 Billion** (Alibaba Group FY2025 Revenue est.) |
| **[Oracle Cloud Compute](https://www.oracle.com/cloud/compute/)** | High-performance enterprise cloud featuring flexible OCPU/RAM ratios and generous Always Free ARM shapes. | **VM.Standard.A1.Flex** (1 OCPU, 6 GiB): **$0.01/hour** (~$7.20/month). **VM.Standard.E4.Flex** (1 OCPU, 16 GiB): **$0.025/hour**. | **Always Free**: **4 Arm Ampere A1 cores + 24 GB RAM** (up to 4 VMs) + 2 AMD VMs + 200 GB storage. Never expires. | **~$53 Billion** (Oracle FY2025 Revenue) |
| **[Linode (Akamai)](https://www.linode.com/pricing/)** | Developer-centric cloud infrastructure now backed by Akamai's global edge network, featuring flat monthly pricing. | **Linode 2 GB** (1 vCPU, 2 GiB, 50 GB SSD): **$12/month** (~$0.018/hour). **Linode 4 GB**: **$24/month**. | **$100 credit for 60 days** (new user trial). No perpetual free tier. | **~$4 Billion** (Akamai FY2025 Revenue) |
| **[OVHcloud](https://www.ovhcloud.com/en/public-cloud/)** | Leading European cloud provider offering GDPR-compliant public cloud instances, bare metal servers, and predictable billing. | **B3-8** (2 vCPU, 8 GiB): **~€0.045/hour** (~€32/month). Savings plans offer up to 30% discount. | **€100 credit for 30 days** (new user trial). No perpetual free tier. | **~$1 Billion** (OVHcloud / Iliad Group est.) |
| **[DigitalOcean Droplets](https://www.digitalocean.com/pricing/droplets)** | Simplicity-first developer cloud featuring fast instance spin-up, predictable pricing, managed Kubernetes, and Droplets. | **Basic Droplet** (1 vCPU, 1 GiB, 25 GB SSD, 1 TB transfer): **$6/month** (~$0.0089/hour). | **$200 credit for 60 days** (new user trial). No perpetual free tier. | **~$700 Million** (Public: DOCN ARR) |
| **[Vultr Compute](https://www.vultr.com/pricing/)** | High-performance independent cloud with 32+ worldwide data center locations, NVMe storage, and bare metal instances. | **Cloud Compute** (1 vCPU, 1 GiB, 25 GB NVMe, 1 TB transfer): **$5/month** (~$0.007/hour). | **$100–$300 credit for 14–30 days** (promotional trial). No perpetual free tier. | **~$500 Million** (Private est. ARR) |
| **[Hetzner Cloud](https://www.hetzner.com/cloud)** | European provider known for lowest price-per-core ratio, NVMe block storage, and high monthly bandwidth inclusion. | **CAX11 ARM** (2 vCPU, 4 GiB, 40 GB NVMe): **~€4.35/month**. **CX23 x86**: **~€5.99/month**. | **€20 credit for 14 days** (new user trial). No perpetual free tier. | **~$100 Million** (Private est. Revenue) |

---

## 🔓 Open-Source GitHub Projects

Open-source cloud compute platforms provide private cloud virtualization, hybrid cloud orchestration, hyperconverged infrastructure (HCI), and Kubernetes-native VM runtimes.

Projects are sorted below by **GitHub_Stars_Count** (descending).

| Repository & Project | Description & Details | License | GitHub_Stars |
| :--- | :--- | :--- | :--- |
| **[OpenStack](https://github.com/openstack)** | **Dominant open-source IaaS cloud framework.** Features modular components (Nova compute, Neutron networking, Cinder block storage, Keystone identity). | Apache-2.0 | [![OpenStack Stars](https://img.shields.io/badge/OpenStack-25,000+-red?style=social&logo=github)](https://github.com/openstack) |
| **[Terraform](https://github.com/hashicorp/terraform)** | **Industry-standard Infrastructure-as-Code (IaC)** tool for declaratively provisioning and managing multi-cloud compute resources across AWS, Azure, GCP, and OpenStack. | BSL 1.1 | [![Terraform Stars](https://img.shields.io/github/stars/hashicorp/terraform?style=social&color=white)](https://github.com/hashicorp/terraform/stargazers) |
| **[KubeVirt](https://github.com/kubevirt/kubevirt)** | **Kubernetes-native virtualization extension.** Runs traditional virtual machine workloads directly inside Kubernetes pods alongside containerized services. | Apache-2.0 | [![KubeVirt Stars](https://img.shields.io/github/stars/kubevirt/kubevirt?style=social&color=white)](https://github.com/kubevirt/kubevirt/stargazers) |
| **[OpenTofu](https://github.com/opentofu/opentofu)** | **Open-source community fork of Terraform** managed by the Linux Foundation. Provides reliable multi-cloud infrastructure provisioning without license restrictions. | Apache-2.0 | [![OpenTofu Stars](https://img.shields.io/github/stars/opentofu/opentofu?style=social&color=white)](https://github.com/opentofu/opentofu/stargazers) |
| **[Cloud Foundry](https://github.com/cloudfoundry)** | **Multi-cloud Application Platform-as-a-Service (PaaS)** and container runtime engine that abstracts underlying IaaS providers for enterprise developers. | Apache-2.0 | [![Cloud Foundry Stars](https://img.shields.io/badge/CloudFoundry-10,000+-blue?style=social&logo=github)](https://github.com/cloudfoundry) |
| **[Harvester](https://github.com/harvester/harvester)** | **Open-source Hyperconverged Infrastructure (HCI)** platform built on Kubernetes, KubeVirt, and Longhorn. Modern open alternative to VMware vSphere. | Apache-2.0 | [![Harvester Stars](https://img.shields.io/github/stars/harvester/harvester?style=social&color=white)](https://github.com/harvester/harvester/stargazers) |
| **[Proxmox VE (Manager)](https://github.com/proxmox/pve-manager)** | **Turnkey open-source enterprise virtualization suite.** Combines KVM hypervisor and LXC containers with web management interface, ZFS, and Ceph storage. | AGPL-3.0 | [![Proxmox Stars](https://img.shields.io/github/stars/proxmox/pve-manager?style=social&color=white)](https://github.com/proxmox/pve-manager/stargazers) |
| **[Apache CloudStack](https://github.com/apache/cloudstack)** | **Turnkey, high-availability open-source IaaS platform.** Designed for managing large networks of virtual machines with low operational complexity. | Apache-2.0 | [![CloudStack Stars](https://img.shields.io/github/stars/apache/cloudstack?style=social&color=white)](https://github.com/apache/cloudstack/stargazers) |
| **[Cloudify](https://github.com/cloudify-cosmo)** | **Multi-cloud orchestration and environment-as-a-service engine.** Automates full lifecycle management of cloud applications across hybrid environments. | Apache-2.0 | [![Cloudify Stars](https://img.shields.io/badge/Cloudify-1,500+-blue?style=social&logo=github)](https://github.com/cloudify-cosmo) |
| **[OpenNebula](https://github.com/OpenNebula/one)** | **Simple yet powerful cloud management platform** for orchestrating KVM virtual machines, edge clusters, and Kubernetes deployments without vendor lock-in. | Apache-2.0 | [![OpenNebula Stars](https://img.shields.io/github/stars/OpenNebula/one?style=social&color=white)](https://github.com/OpenNebula/one/stargazers) |
| **[Apache jclouds](https://github.com/apache/jclouds)** | **Multi-cloud abstraction toolkit for Java and Clojure.** Gives developers portable control over compute instances and blob storage across cloud vendors. | Apache-2.0 | [![jclouds Stars](https://img.shields.io/github/stars/apache/jclouds?style=social&color=white)](https://github.com/apache/jclouds/stargazers) |

---

## 🤝 How to Contribute

Contributions are welcome! Help us maintain the most comprehensive guide to Cloud Compute and IaaS:

1. **Fork** this repository.
2. Add your suggested SaaS provider or open-source repo to `README.md`.
3. Follow the established table schema (include description, specific pricing/stars, and direct links).
4. Submit a **Pull Request** with a brief overview of the added resource.

Please ensure all added entries refer to active projects or production-grade IaaS products.

---

## 💖 Support & Sponsorship

If you find this repository helpful for your cloud engineering work, DevOps research, or technical evaluation, consider supporting the project!

- 🌟 **Star** this repository on GitHub to increase visibility.
- 🔀 **Fork** and share it with your cloud architecture team or engineering colleagues.
- ☕ **Buy me a coffee / Sponsor**: If you'd like to support ongoing maintenance of awesome lists, consider becoming a sponsor:
  
  [👉 **Sponsor on GitHub Sponsors** 👈](https://github.com/sponsors/ishandutta2007)

Thank you for being part of the open-source cloud community!

---

## ⭐ Star History

[![Star History Chart](https://star-history.dera.page/svg?repos=ishandutta2007/Awesome-Cloud-Compute-IaaS&type=date&legend=top-left)](https://star-history.dera.page/#ishandutta2007/Awesome-Cloud-Compute-IaaS&type=date&legend=top-left)

---

## ⚠️ Disclaimer

- This list is **community-curated** for educational and research purposes.
- All SaaS pricing figures and open-source star metrics are accurate as of **October 2026** and subject to change by respective vendors and maintainers.
- Cloud security, compliance, and workload isolation remain the responsibility of deploying teams.

---

<p align="center">
  <b>Curated with ❤️ for DevOps Engineers, Cloud Architects, and Infrastructure Developers worldwide.</b>
</p>
