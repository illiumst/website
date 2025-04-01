---
layout: single
title: "LMU DevOps Admin"
categories: projects
tags: devops kubernetes server-administration infrastructure
excerpt: "Managed LMU chair IT: Kubernetes, CI/CD, automation (2018-2023)."
header:
  teaser: /assets/images/projects/arch.png # Corrected path
role: System Administrator, DevOps Engineer, Network Administrator
skills: Kubernetes (K3S), Ansible, Docker, CI/CD (GitLab CI, Argo CD), GitOps, Linux Server Administration (Debian, Arch), Networking (Traefik, WireGuard), Virtualization (Hyper-V), Storage (ZFS, Longhorn), Monitoring (WandB), Infrastructure as Code (IaC)
---

![Arch Linux Logo](/assets/images/projects/arch.png){: .align-left style="padding:0.1em; width:5em" alt="Arch Linux Logo"}
During my tenure at the LMU Chair for Mobile and Distributed Systems, alongside my research activities, I assumed responsibility for the ongoing maintenance of the group's IT infrastructure. This encompassed Linux workstations, Windows Server-based hypervisors, Linux file servers (utilizing ZFS), and core network services.

---

**Role:** IT Infrastructure & DevOps Lead (Informal)<br>
**Affiliation:** Chair for Mobile and Distributed Systems, LMU Munich<br>
**Duration:** 2018 - 2023 (Concurrent with Research Role)<br>
**Objective:** Continious maintenance of IT infrastructure

---

**Key Initiatives & Achievements:**

*   **Infrastructure as Code & Orchestration:**
    *   Leveraged **Ansible** extensively for automated configuration management and orchestration across a heterogeneous environment, ensuring consistency and reducing manual effort in managing diverse operating systems (Debian, Arch Linux, Windows), hardware configurations, and software libraries.

*   **Containerization & Kubernetes Migration:**
    *   Spearheaded the migration of numerous internal services (including web applications, databases, and research tools) from traditional VMs and bare-metal deployments to a **Kubernetes (K3S)** cluster. This enhanced scalability, resilience, and resource utilization.
    *   Implemented **Longhorn** for persistent, distributed block storage within the Kubernetes cluster.

*   **DevOps & GitOps Implementation:**
    *   Established a modern DevOps workflow centered around a self-hosted **GitLab** instance, utilizing **GitLab CI** for automated testing and container building.
    *   Implemented **Argo CD** for GitOps-based continuous deployment to the Kubernetes cluster, ensuring declarative state management and automated synchronization.
    *   Managed sensitive information using **Sealed Secrets** for secure secret handling within the GitOps workflow.

*   **Networking & Security:**
    *   Configured **Traefik** as the primary reverse proxy and ingress controller for the Kubernetes cluster, automating routing, service discovery, and TLS certificate management.
    *   Implemented and managed a **WireGuard** VPN server to provide secure remote access for chair members to internal resources.

*   **ML Workflow Optimization:**
    *   Re-architected the execution environment for machine learning experiments. Transitioned from managing dependencies directly on workstations or via a less reliable SLURM setup to a containerized approach using **Docker**.
    *   Utilized the self-hosted **GitLab Container Registry** for storing ML environment images.

---

**Outcomes & Philosophy:**

This hands-on role provided deep practical experience in modern system administration, networking, Infrastructure as Code (IaC), and cloud-native technologies within an academic research setting. It fostered my preference for minimalist, reproducible, and microservice-oriented architectures. These principles and skills are actively applied in my personal projects, including the self-hosting and management of this website and various other containerized services.

A more comprehensive list of the technologies I work with can be found on the [About Me](/about/) page.