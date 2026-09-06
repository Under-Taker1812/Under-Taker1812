<h1 align="center">Hi 👋, I'm Huỳnh Ân</h1>

<p align="center">
  <img src="https://readme-typing-svg.demolab.com/?font=Fira+Code&size=18&pause=1200&color=7AA2F7&center=true&vCenter=true&width=650&lines=DevOps+%2F+Platform+trainee;Running+production+infra+on+real+hardware;Proxmox+%7C+Ceph+%7C+Kubernetes+%7C+Ansible" alt="typing" />
</p>

<table width="100%">
  <tr>
    <td width="60%" valign="top">
      <p>2nd-year CS student at UIT, Vietnam. I intern at a company and run production infrastructure on real hardware. When something breaks, I document the root cause and fix it properly.</p>
      <p>
        <img src="https://visitor-badge.laobi.icu/badge?page_id=Under-Taker1812.Under-Taker1812&right_color=7AA2F7&left_color=1a1b26" alt="profile views" />
        <a href="https://github.com/Under-Taker1812">
          <img src="https://img.shields.io/github/followers/Under-Taker1812?style=flat-square&logo=github&label=followers&color=7AA2F7&labelColor=1a1b26" alt="GitHub followers" />
        </a>
      </p>
      <p>
        <a href="https://www.linkedin.com/in/REPLACE_ME/" target="_blank">
          <img src="https://img.shields.io/static/v1?message=LinkedIn&logo=linkedin&label=&color=0077B5&logoColor=white&style=for-the-badge" height="24" alt="linkedin" />
        </a>
        <a href="mailto:24560064@gm.uit.edu.vn">
          <img src="https://img.shields.io/static/v1?message=Email&logo=gmail&label=&color=D14836&logoColor=white&style=for-the-badge" height="24" alt="email" />
        </a>
        <a href="https://www.facebook.com/share/1CcW5eCW6C/" target="_blank">
          <img src="https://img.shields.io/static/v1?message=Facebook&logo=facebook&label=&color=1877F2&logoColor=white&style=for-the-badge" height="24" alt="facebook" />
        </a>
        <img src="https://img.shields.io/static/v1?message=huynhan4210&logo=discord&label=Discord&color=7289DA&logoColor=white&style=for-the-badge" height="24" alt="discord" />
      </p>
    </td>
    <td width="40%" valign="top" align="center">
      <!--
        TODO: this widget needs YOUR OAuth authorization, a public profile link isn't enough.
        1. Go to https://spotify-recently-played.jeffreyca.workers.dev
        2. Click "Connect with Spotify" and log in with your own account
        3. Pick theme "Tokyo Night", Tracks = 5
        4. Click "Copy snippet" and paste it here, replacing this whole <td>...</td> block
      -->
      <img src="https://img.shields.io/badge/Spotify-connect%20your%20account%20first-1DB954?style=for-the-badge&logo=spotify&logoColor=white" alt="spotify placeholder" />
    </td>
  </tr>
</table>

---

<table width="100%">
  <thead>
    <tr><th align="left">My Journey</th></tr>
  </thead>
  <tbody>
    <tr>
      <td>
        <p align="left">I run a 4-node Proxmox cluster with Ceph storage (8 OSDs, ~7TB) and a Rancher/RKE2 Kubernetes cluster on physical hardware during my internship. I've debugged Calico VTEP conflicts and recovered etcd from a NOSPACE alarm. Prometheus and Grafana cover monitoring for the whole stack. Right now I'm studying for the CKA and AWS SAA to put a certification behind work I already do.</p>
        <p align="left">
          <img src="https://img.shields.io/badge/NOW-CKA%20%2B%20AWS%20SAA-9ECE6A?style=for-the-badge&logo=kubernetes&logoColor=1a1b26" alt="now" />
        </p>
        <p align="right">My Ansible playbooks deploy that cluster end to end — 14 playbooks under one site.yml, including automated teardown and rebuild. Networking is my strongest starting point from school: VLANs, OSPF, RIP, ACLs, NAT. CCNA, Terraform, and a service mesh lab are next.</p>
        <p align="right">
          <img src="https://img.shields.io/badge/NEXT-CCNA%20%7C%20Terraform%20%7C%20Service%20Mesh-7AA2F7?style=for-the-badge&logo=terraform&logoColor=1a1b26" alt="next" />
        </p>
        <p align="left">I'm building toward two roles at once: Cloud Security Engineer and Platform Engineer. Both need the same Kubernetes and cloud foundation before they split — CKS and AWS Security Specialty on one side, Terraform and GitOps on the other.</p>
        <p align="left">
          <img src="https://img.shields.io/badge/GOAL-Cloud%20Security%20%26%20Platform%20Engineer-BB9AF7?style=for-the-badge&logo=cloudflare&logoColor=1a1b26" alt="goal" />
        </p>
      </td>
    </tr>
  </tbody>
</table>

---

### 🛠️ Stack I run daily

<p align="center">
  <a href="https://skillicons.dev">
    <img src="https://skillicons.dev/icons?i=kubernetes,ansible,aws,docker,grafana,prometheus,elasticsearch,git,github,py,linux,ubuntu,bash,powershell,nginx,windows&perline=16" alt="Tech Stack Icons" />
  </a>
</p>

**No icon exists for these, but I run them daily:** Proxmox (4-node hyperconverged cluster), Ceph (distributed storage, CRUSH, monmap recovery), Rancher/RKE2, Calico CNI, etcd, Ceph CSI RBD, Cisco networking (VLAN/OSPF/RIP/ACL/NAT), Wazuh SIEM, OSSEC HIDS, ssacli (HP Smart Array RAID).

### 🗺️ Where I stand

> GitHub does not render Mermaid `mindmap` diagrams. This is a `graph` with subgraphs instead.

```mermaid
graph LR
    ME(("Huỳnh Ân")):::me

    subgraph INFRA[" Infra "]
        direction TB
        PROXMOX["Proxmox<br/>4-node HCI"]:::prod
        CEPH["Ceph<br/>8 OSD · ~7TB"]:::prod
        RANCHER["Rancher / RKE2<br/>1 CP + 3 workers"]:::prod
    end

    subgraph NET[" Network "]
        direction TB
        CALICO["Calico CNI<br/>VTEP & nftables"]:::prod
        CISCO["VLAN / OSPF / ACL / NAT"]:::prod
        VPN["VPN & NGINX proxy"]:::prod
    end

    subgraph OBS[" Observability "]
        direction TB
        PROM["Prometheus"]:::prod
        GRAF["Grafana"]:::prod
        ALERT["AlertManager"]:::prod
        ELK["Elasticsearch / Kibana / Fluent-bit"]:::prod
    end

    subgraph AUTO[" Automation "]
        direction TB
        ANSIBLE["Ansible<br/>14 playbooks, site.yml"]:::prod
        PYTHON["Python scripting"]:::prod
    end

    subgraph CLOUD[" Cloud "]
        direction TB
        AWS["AWS<br/>EC2 / RDS / CI-CD"]:::prod
    end

    subgraph SEC[" Security "]
        direction TB
        WAZUH["Wazuh SIEM / OSSEC HIDS"]:::prod
        CKS["CKS track<br/>next certification"]:::plan
    end

    ME --> INFRA
    ME --> NET
    ME --> OBS
    ME --> AUTO
    ME --> CLOUD
    ME --> SEC

    classDef me fill:#7aa2f7,stroke:#1a1b26,color:#1a1b26,font-weight:bold,font-size:16px
    classDef prod fill:#9ece6a,stroke:#1a1b26,color:#1a1b26
    classDef plan fill:#565f89,stroke:#1a1b26,color:#ffffff
```

---

### 🎓 Certifications

<!-- Once you earn a cert, go to its Credly badge page > Share > Embed, and swap the image/link below. -->

<p align="center">
  <img src="https://img.shields.io/badge/CKA-not%20earned%20yet-565F89?style=for-the-badge&logo=kubernetes&logoColor=white" alt="CKA placeholder" />
  <img src="https://img.shields.io/badge/AWS%20SAA-not%20earned%20yet-565F89?style=for-the-badge&logo=amazonaws&logoColor=white" alt="AWS SAA placeholder" />
  <img src="https://img.shields.io/badge/CKS-not%20earned%20yet-565F89?style=for-the-badge&logo=kubernetes&logoColor=white" alt="CKS placeholder" />
</p>

---

### 📌 Featured project

[![proxmox-lab-portfolio](https://github-readme-stats.vercel.app/api/pin/?username=Under-Taker1812&repo=proxmox-lab-portfolio&theme=tokyonight&hide_border=true)](https://github.com/Under-Taker1812/proxmox-lab-portfolio)

---

### 📊 GitHub Stats

<table width="100%">
  <tr>
    <td width="50%"><img src="https://github-readme-stats.vercel.app/api?username=Under-Taker1812&show_icons=true&theme=tokyonight&hide_border=true" alt="GitHub Stats" width="100%" /></td>
    <td width="50%"><img src="https://streak-stats.demolab.com/?user=Under-Taker1812&theme=tokyonight&hide_border=true" alt="GitHub Streak" width="100%" /></td>
  </tr>
</table>
