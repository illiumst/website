---
layout: single
title:  "Linux Server Administration"
categories: projects server_admin unix
excerpt: "Linux Server Administration (Workstations and Web)"
header:
  teaser: assets/images/projects/arch.png
---
![logo](\assets\images\projects\arch.png){: .align-left style="padding:0.1em; width:5em"}
During my time at the Mobile Distributed Systems Chair, I also supported my colleagues regarding the setup and maintenance of our workstations, the Windows server hypervisor, our Linux file server, and our networking infrastructure.
We orchestrated and utilized multiple systems with varying operating systems, hardware, driver versions, and libraries (damn you CUDA), mostly through Ansible.

Most recently transferred a major partition of or services to Kubernetes (K3S) while setting up a complete tool chain including Longhorn, Argo CD, Sealed Secrets, and GitLab. For ingress and egress, we set up Traefik as our fully automated proxy manager. 
This way, we could differentiate between routes through different virtual networks for clients within our networks and external users, i.e., colleagues in the home office or students.
Crossing network borders was possible through a self-hosted WireGuard jump-host, which could also be utilized as our full-fledged VPN when traveling aboard.
This way, the whole team could access our ZFS-file server from anywhere.

Starting with self-scripted ML runs on non-reliable SLURM infrastructure (pool PCs could be turned off or used by students, which killed the SLURM agent at any time), I slowly transitioned to runs on individual, high-performance workstations.
Lately, those units were automated by weights-and-biases (WandB), which automatically runs experiments in pre-defined Docker containers; for that, we utilized our self-hosted registry through GitLab.

All in all, I learned a lot about Linux server administration, networking, code-as-infrastructure, and the spirit of the cloud native approach.
Nowadays, I thoroughly enjoy the `make your requirements less dumb` approach to things, moving from central services to a bunch of problem-specific (self-hosted) microservices.
Moreover, I really like to build systems from the ground up with only the necessary elements on top of a rolling release distribution (Arch-Linux-based).

I took some concepts into my `home lab`, where I now self-host most of my services, including this website. Isn't that cool? :cool: More of the tech stack I encountered on my journey is listed [here](/about).
