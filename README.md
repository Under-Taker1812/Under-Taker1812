<h1 align="center">Hi 👋, I'm Huỳnh Ân</h1>

<p align="center">
  <img src="https://readme-typing-svg.demolab.com/?font=Fira+Code&size=18&pause=1200&color=7AA2F7&center=true&vCenter=true&width=650&lines=DevOps+%2F+Platform+trainee+today;Aspiring+Cloud+Security+Engineer+tomorrow;Running+real+infra+on+physical+hardware" alt="typing" />
</p>

<table width="100%">
  <tr>
    <td width="60%" valign="top">
      <p>2nd-year CS student @ UIT, Vietnam — interning and building production-grade infrastructure on real hardware, not just tutorial labs. I break things, write down why, and fix them properly.</p>
      <p>
        <img src="https://visitor-badge.laobi.icu/badge?page_id=Under-Taker1812.Under-Taker1812&right_color=7AA2F7&left_color=1a1b26" alt="profile views" />
        <a href="https://github.com/Under-Taker1812">
          <img src="https://img.shields.io/github/followers/Under-Taker1812?style=flat-square&logo=github&label=followers&color=7AA2F7&labelColor=1a1b26" alt="GitHub followers" />
        </a>
      </p>
      <p>
        <!-- Replace with your real links -->
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
        <p align="left">I'm on a journey to become a <b>DevOps / Platform engineer</b> who can build, automate, and secure real systems — not just pass exams. Turning a 3am production incident into a documented runbook so it never repeats is more satisfying to me than any tutorial checkbox.</p>
        <p align="left">
          <img src="https://img.shields.io/badge/NOW-CKA%20%2B%20AWS%20SAA-9ECE6A?style=for-the-badge&logo=kubernetes&logoColor=1a1b26" alt="now" />
        </p>
        <p align="right">Right now I'm hands-deep in real hardware: a <b>4-node Proxmox cluster</b>, <b>Ceph</b> distributed storage, and a <b>Rancher/RKE2</b> cluster running production-style workloads during my internship. Every bug becomes a written case study, not a forgotten Slack thread.</p>
        <p align="right">
          <img src="https://img.shields.io/badge/NEXT-CCNA%20%7C%20Terraform%20%7C%20Service%20Mesh-7AA2F7?style=for-the-badge&logo=terraform&logoColor=1a1b26" alt="next" />
        </p>
        <p align="left">Longer term I'm building toward two tracks at once — <b>Cloud Security Engineer</b> and <b>Platform Engineer</b> — since both share the same Kubernetes/cloud foundation before splitting into specialties.</p>
        <p align="left">
          <img src="https://img.shields.io/badge/GOAL-Cloud%20Security%20%26%20Platform%20Engineer-BB9AF7?style=for-the-badge&logo=cloudflare&logoColor=1a1b26" alt="goal" />
        </p>
      </td>
    </tr>
  </tbody>
</table>

---

### 🗺️ Where I stand

> GitHub doesn't render Mermaid `mindmap` diagrams (platform limitation, verified) — this is a `graph` with clustered subgraphs instead, which renders reliably.

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
    end

    subgraph OBS[" Observability "]
        direction TB
        PROM["Prometheus"]:::prod
        GRAF["Grafana"]:::prod
        ALERT["AlertManager"]:::prod
    end

    subgraph AUTO[" Automation "]
        direction TB
        ANSIBLE["Ansible<br/>in progress"]:::learn
    end

    subgraph CLOUD[" Cloud "]
        direction TB
        AWS["AWS<br/>~30%"]:::learn
    end

    subgraph SEC[" Security "]
        direction TB
        CKS["CKS track<br/>roadmap"]:::plan
    end

    ME --> INFRA
    ME --> NET
    ME --> OBS
    ME --> AUTO
    ME --> CLOUD
    ME --> SEC

    classDef me fill:#7aa2f7,stroke:#1a1b26,color:#1a1b26,font-weight:bold,font-size:16px
    classDef prod fill:#9ece6a,stroke:#1a1b26,color:#1a1b26
    classDef learn fill:#ff9e64,stroke:#1a1b26,color:#1a1b26
    classDef plan fill:#565f89,stroke:#1a1b26,color:#ffffff
```

---

### 🎓 Certifications

<!-- Once you earn a cert, go to its Credly badge page > Share > Embed, and swap the image/link below. Keeping these as "not earned yet" until then — no faking. -->

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
