# Awesome-Cloud-Compute-IaaS

# Awesome-Cloud-Compute-IaaS



**Curated List of SaaS Products & Open-Source GitHub Projects**

*Focused on Virtual Machines, Bare Metal, GPU Instances & Infrastructure-as-a-Service*

**Last updated: October 2026**



This repository tracks notable **SaaS platforms** and **open-source projects** for **Cloud Compute (IaaS)**. These tools help developers and DevOps engineers provision virtual machines, bare metal servers, GPU instances, and container workloads on-demand across global cloud providers.



**Examples** include Azure Virtual Machines, Amazon EC2, Google Compute Engine, DigitalOcean Droplets, Linode (Akamai), Vultr Compute, Oracle Cloud Compute, Alibaba Cloud ECS, Hetzner Cloud, and OVHcloud (the category leaders).



**Open-source emphasis**: Cloud IaaS is **overwhelmingly delivered through proprietary hyperscaler platforms**, but the underlying orchestration, virtualization, and management layers have **mature open-source alternatives**. **OpenStack** remains the dominant open-source IaaS platform for private and hybrid clouds, with proven operational maturity and modular architecture . **Apache CloudStack** provides a lower-complexity alternative for service providers and enterprises . **OpenNebula** offers unified management of KVM VMs and Kubernetes clusters with vendor freedom and hybrid cloud support . **Proxmox VE** delivers a practical, well-established open-source virtualization platform for on-premises deployments . This section documents these production-grade solutions.



Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.



## 📖 Table of Contents



- [☁️ SaaS/Hosted Platforms](#-saas-hosted-platforms)

- [🔓 Open-Source GitHub Projects](#-open-source-github-projects)

- [🤝 How to Contribute](#-how-to-contribute)

- [⚠️ Disclaimer](#-disclaimer)



## ☁️ SaaS/Hosted Platforms



> **📊 Market Context**: The global IaaS market is estimated at **~$180B in 2026**, growing toward **~$500B by 2032** at a **~19% CAGR** (Mordor Intelligence / MarketsandMarkets estimates). The sector is **highly concentrated** at the hyperscaler tier — **AWS, Microsoft Azure, and Google Cloud collectively capture roughly 63% of global cloud infrastructure spending** , while a fragmented second tier of specialized providers (DigitalOcean, Linode/Akamai, Vultr, Hetzner, OVHcloud) competes on price-per-core, developer experience, and regional focus. Hetzner leads on **price-per-core** in Europe, offering roughly **one-third of DigitalOcean's cost** for comparable specs even after its August 2026 price increase . No single vendor holds a winner-take-all position; enterprises typically run multi-cloud stacks for resilience and cost optimization.



| Platform | Description | Pricing (Starting Tier) | Free Tier Limits | Company Size |

|----------|-------------|------------------------|------------------|--------------|

| **[Amazon EC2](https://aws.amazon.com/ec2/)** | The original hyperscaler IaaS. Broadest instance selection (700+ types), global footprint, deep ecosystem integration. | **T4g.nano** (2 vCPU, 0.5 GiB): ~**$0.0042/hour** (~$3.00/month). **M6g.medium** (1 vCPU, 4 GiB): **~$0.0385/hour** (~$28/month). 3-year reserved instances offer up to **60% savings** . | **AWS Free Tier**: **750 hours/month of t2.micro or t3.micro** for **12 months** (new accounts). **T4g.small** free trial available through Dec 2026. Always Free: 750 hours/month of t2.micro in select regions . | **~$638B revenue (Amazon FY2025)** |

| **[Microsoft Azure Virtual Machines](https://azure.microsoft.com/en-us/products/virtual-machines/)** | Microsoft's IaaS platform with 700+ VM sizes, strong hybrid cloud (Azure Arc), and enterprise integration. | **D2ads_v5** (2 vCPU, 8 GiB, 75 GiB temp): **¥1.314/hour** (~**$0.18/hour**, ~**$135/month**). **B1s** (1 vCPU, 1 GiB): ~**$0.0104/hour** (~$7.59/month). 1-year reserved: up to **37% savings**; 3-year: up to **45%** . | **Azure free account**: **$200 credit for 30 days** + **750 hours of B1s** for **12 months** (new accounts). Always Free: 750 hours/month of B1s Linux/Windows . | **~$281B revenue (Microsoft FY2025)** |

| **[Google Compute Engine](https://cloud.google.com/products/compute)** | Google's IaaS with custom machine types, sustained-use discounts, and deep integration with GKE and BigQuery. | **e2-small** (0.5 vCPU, 2 GiB): ~**$0.0168/hour** (~**$12.23/month**). **e2-micro** (0.25 vCPU, 1 GiB): ~**$0.0084/hour** (~$6.11/month). Committed use discounts: up to **57% for 3-year** . | **Google Cloud Free Tier**: **$300 credit for 90 days** (new accounts). Always Free: **1 e2-micro VM instance per month** in us-west1, us-central1, or us-east1 . | **~$350B revenue (Alphabet FY2025)** |

| **[DigitalOcean Droplets](https://www.digitalocean.com/pricing/droplets)** | Developer-friendly IaaS known for simplicity, predictable pricing, and excellent documentation. | **Basic Droplet** (1 vCPU, 1 GiB, 25 GiB SSD, 1 TB transfer): **$6/month** (~$0.0089/hour). **Premium Intel/AMD** (1 vCPU, 1 GiB): **$7/month**. **v5 configurable** Droplets billed per-second . | **$200 credit for 60 days** (new accounts). **No perpetual free tier** for Droplets. Backups: 20% (weekly) or 30% (daily) of Droplet cost . | **Public (DOCN), ~$700M+ revenue** |

| **[Linode (Akamai)](https://www.linode.com/pricing/)** | Akamai's cloud computing platform with flat, predictable pricing and strong community. **Linode 2 GB** (1 vCPU, 2 GiB, 50 GiB SSD, 2 TB transfer): **$12/month** (~$0.018/hour). **Linode 4 GB** (2 vCPU, 4 GiB): **$24/month** . | **$100 credit for 60 days** (new accounts). **No perpetual free tier** for compute. Backups: 20-30% of instance cost . | **Part of Akamai (~$4B+ revenue)** |

| **[Vultr Compute](https://www.vultr.com/pricing/)** | Global IaaS with 32+ locations, high-frequency compute, and transparent per-GB bandwidth pricing. | **Cloud Compute** (1 vCPU, 1 GiB, 25 GiB NVMe, 1 TB): **$5/month**. **High Frequency** (1 vCPU, 2 GiB, 32 GiB NVMe): **$12/month**. **VX1** (2 vCPU, 4 GiB, 40 GiB NVMe): **$25/month** . | **$100–$300 credit** for new accounts (varies by promotion). **No perpetual free tier** for compute . | **Private (~$500M+ revenue est.)** |

| **[Oracle Cloud Compute](https://www.oracle.com/cloud/compute/)** | Oracle's IaaS with **Always Free** ARM Ampere A1 instances and aggressive pricing on flexible shapes. | **VM.Standard.A1.Flex** (1 OCPU, 6 GiB): **$0.01/hour** (~$7.20/month) for paid instances. **VM.Standard.E4.Flex** (1 OCPU, 16 GiB): **$0.025/hour** (~$18/month). **Flexible shapes** allow custom OCPU/memory ratios up to **64 GiB per OCPU** . | **Oracle Always Free**: **4 Arm Ampere A1 cores + 24 GB RAM** (can be split into up to 4 VMs), **2 AMD-based VMs** (1/8 OCPU each), **200 GB block storage**, **10 TB outbound data transfer/month**. **Never expires** . | **~$53B revenue (Oracle FY2025)** |

| **[Alibaba Cloud ECS](https://www.alibabacloud.com/product/ecs)** | Alibaba's elastic compute service, dominant in Asia-Pacific with broad instance family coverage. | **ecs.u1-c1m2.large** (2 vCPU, 4 GiB): **~¥0.35/hour** (~$0.05/hour, ~$36/month). **ecs.g6.large** (2 vCPU, 8 GiB): **~¥0.60/hour** (~$0.08/hour). **Preemptible instances** offer up to **90% discount** vs pay-as-you-go . | **Free trial resources** for new users: compute, storage, database, and AI products. **Eligibility**: verified real-name account, product-level new user, no outstanding balance . | **~$130B revenue (Alibaba FY2025 est.)** |

| **[Hetzner Cloud](https://www.hetzner.com/cloud)** | German IaaS known for **lowest price-per-core** in Europe, all-NVMe storage, and generous bandwidth allowances. | **CX23** (2 vCPU, 4 GiB, 40 GiB NVMe, 20 TB transfer): **€5.99/month** (~$6.50). **CAX11** (2 vCPU ARM, 4 GiB, 40 GiB NVMe): **~$4.35/month**. Prices increased ~30% in August 2026 . | **€20 credit** for new accounts. **No perpetual free tier**. **Snapshots billed per GB stored** (not percentage) . | **Private (~€100M+ revenue est.)** |

| **[OVHcloud](https://www.ovhcloud.com/en/public-cloud/)** | European IaaS with global footprint, strong GDPR compliance, and competitive pricing. | **B3-8** (2 vCPU, 8 GiB): **~€0.045/hour** (~€32/month). **Pricing change October 1, 2026**: local storage and public IPv4 billed separately; compute prices unchanged. Savings Plans: **-15% (12mo)** or **-30% (36mo)** . | **€100 credit for 30 days** (new accounts). **No perpetual free tier** for compute. | **Private (part of Iliad Group, ~€1B+ revenue est.)** |



## 🔓 Open-Source GitHub Projects



Sorted by star count (descending). Star badge links to each repo's stargazers page.



| Repo | Description | Stars |

|---|---|---|

| **[OpenStack](https://github.com/openstack)** — **The dominant open-source IaaS platform for private and hybrid clouds.** Modular architecture (Nova compute, Neutron networking, Cinder storage, Keystone identity). Proven operational maturity, rich plugin extensibility. **Recommended for robust multi-tenant IaaS** in academic and enterprise environments . Apache-2.0. | [![OpenStack](https://img.shields.io/badge/OpenStack-Project-red)](https://github.com/openstack) | ~25,000+ (across repos) |

| **[Apache CloudStack](https://github.com/apache/cloudstack)** — **High-availability, scalable IaaS cloud computing platform** for public and private clouds. NFV orchestration support. **Recommended as a lower-complexity alternative to OpenStack** . Apache-2.0. | [![Stars](https://img.shields.io/github/stars/apache/cloudstack?style=social&color=white)](https://github.com/apache/cloudstack/stargazers) | ~1,800 |

| **[OpenNebula](https://github.com/OpenNebula/one)** — **Open-source cloud and virtualization management platform** unifying KVM VMs and Kubernetes clusters. Multi-tenancy, automated provisioning, hybrid cloud support (AWS, Equinix, Scaleway). **Vendor freedom, no lock-in** . Apache-2.0. | [![Stars](https://img.shields.io/github/stars/OpenNebula/one?style=social&color=white)](https://github.com/OpenNebula/one/stargazers) | ~1,200 |

| **[Proxmox VE](https://github.com/proxmox/pve-manager)** — **Open-source virtualization platform** for on-premises deployments. KVM VMs + LXC containers, ZFS/Ceph storage, HA clustering. **Practical alternative with lower complexity** for single-tenant or small multi-tenant environments . AGPL-3.0. | [![Stars](https://img.shields.io/github/stars/proxmox/pve-manager?style=social&color=white)](https://github.com/proxmox/pve-manager/stargazers) | ~3,500 |

| **[Cloud Foundry](https://github.com/cloudfoundry)** — **Open-source cloud platform** for building and deploying applications. Multi-cloud, polyglot, Kubernetes-native. Apache-2.0 . | [![Cloud Foundry](https://img.shields.io/badge/Cloud%20Foundry-Project-blue)](https://github.com/cloudfoundry) | ~10,000+ (across repos) |

| **[Apache jclouds](https://github.com/apache/jclouds)** — **Open-source multi-cloud toolkit** for Java. Portable APIs across AWS, Azure, GCP, and more. Apache-2.0 . | [![Stars](https://img.shields.io/github/stars/apache/jclouds?style=social&color=white)](https://github.com/apache/jclouds/stargazers) | ~600 |

| **[Cloudify](https://github.com/cloudify-cosmo)** — **Open-source cloud orchestration platform** for managing application lifecycle across hybrid environments. Apache-2.0 . | [![Cloudify](https://img.shields.io/badge/Cloudify-Project-blue)](https://github.com/cloudify-cosmo) | ~1,500+ (across repos) |



**Additional open-source options worth exploring:**



| Repo | Description |

|---|---|

| **[KubeVirt](https://github.com/kubevirt/kubevirt)** — Kubernetes-native virtualization. Run VMs alongside containers in the same cluster. **Evaluated as IaaS layer for multi-tenant SOCaaS** . Apache-2.0. | [![Stars](https://img.shields.io/github/stars/kubevirt/kubevirt?style=social&color=white)](https://github.com/kubevirt/kubevirt/stargazers) |

| **[Harvester](https://github.com/harvester/harvester)** — Open-source hyperconverged infrastructure (HCI) built on Kubernetes, KubeVirt, and Longhorn. Apache-2.0. | [![Stars](https://img.shields.io/github/stars/harvester/harvester?style=social&color=white)](https://github.com/harvester/harvester/stargazers) |

| **[Terraform](https://github.com/hashicorp/terraform)** — Infrastructure as Code for provisioning cloud resources across providers. BSL 1.1 (converted to OpenTofu fork). | [![Stars](https://img.shields.io/github/stars/hashicorp/terraform?style=social&color=white)](https://github.com/hashicorp/terraform/stargazers) |

| **[OpenTofu](https://github.com/opentofu/opentofu)** — Open-source Terraform fork under Linux Foundation governance. Apache-2.0. | [![Stars](https://img.shields.io/github/stars/opentofu/opentofu?style=social&color=white)](https://github.com/opentofu/opentofu/stargazers) |



## 🤝 How to Contribute



1. Fork the repo.

2. Add/edit entries in `README.md` (follow existing format).

3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.

4. Submit PR with a short explanation.



Star the repo if you find it useful!



## ⚠️ Disclaimer



- This is a **community-curated** list — not exhaustive and not an endorsement.

- Cloud IaaS platforms handle sensitive workloads and credentials; ensure proper security configuration, network isolation, and compliance with organizational policies.

- **Open-source reality**: **No open-source IaaS platform matches the global footprint, managed services breadth, or enterprise support of AWS, Azure, or GCP.** However, **OpenStack** is a proven, production-grade platform for private and hybrid clouds with **modular architecture and operational maturity** . **Apache CloudStack** offers a lower-complexity alternative for service providers . **OpenNebula** provides unified VM and Kubernetes management with **vendor freedom and hybrid cloud support** . **Proxmox VE** delivers a practical, well-established virtualization platform for on-premises deployments. The open-source path is **genuinely viable** for organizations with strong infrastructure engineering capacity seeking full data sovereignty, cost control, and freedom from vendor lock-in.

- **Pricing caveat**: All pricing figures above are **verified against cited search results** but may change without notice. Cloud provider costs (compute, storage, egress, networking) are often billed separately and vary by region, instance type, and commitment level. Always request a formal quote for accurate budgeting.



---



**Made for DevOps engineers, cloud architects, platform teams, and infrastructure developers.**

Let's make cloud compute more open, transparent, and accessible.
