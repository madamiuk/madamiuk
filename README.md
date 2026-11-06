# 👨‍💻 Mirosław Adamiuk

**Linux System Engineer | Production Infrastructure & Managed Hosting | Automation**

📍 Poland  
💼 [LinkedIn](https://www.linkedin.com/in/miros%C5%82aw-adamiuk-548821222/) · 🌐 [GitHub](https://github.com/madamiuk)

---

## About me

Linux System Engineer and IT infrastructure professional with a career in IT dating back to 2005, including hands-on administration of **production Linux environments**, hosting services, networking, monitoring, virtualization and security.

At Intratel, my day-to-day work included **SUSE Linux Enterprise Server**, production web, email and FTP services, Postfix mail security and delivery troubleshooting, Centreon monitoring, and Linux infrastructure supporting cloud-based customer environments. I also worked with VMware vSphere for Linux VM operations within clearly defined permissions, collaborating with dedicated networking and virtualization teams.

Alongside professional operations experience, I build **personal infrastructure automation labs** using Ansible, Bash, Git, Terraform, Oracle Cloud Infrastructure and CI/CD tools. These projects are learning and engineering work, **not a claim of commercial DevOps experience**.

---

## ⚡ Highlights

- Production Linux administration, primarily **SUSE Linux Enterprise Server**
- Managed hosting operations: **web, email, FTP, DNS and related services**
- Postfix email infrastructure security: **Amavis, Rspamd, SpamAssassin, SPF, DKIM, DMARC**
- Service monitoring, incident investigation and mail delivery troubleshooting
- VMware vSphere: Linux VM operations, test VM provisioning and pre-maintenance snapshots (limited privileges)
- Infrastructure automation labs with **Ansible**
- Fresh-host provisioning for **Debian and RHEL-based systems**
- Java application platforms: **WildFly and Apache Tomcat**
- PostgreSQL provisioning and JDBC/JNDI integration
- CI/CD with **GitHub Actions, Jenkins and GitLab**
- Monitoring with **Centreon, Nagios, Prometheus, Grafana, NRPE and Node Exporter**
- Networking, DNS, routing, firewalls and service troubleshooting
- **SUSE Certified Engineer · CompTIA Security+ · CCNA**

---

## 🛠 Tech Stack

**Linux:** SUSE Linux Enterprise Server · RHEL · Oracle Linux · Debian  
**Automation:** Ansible · Ansible Vault · Bash · Jinja2  
**CI/CD:** GitHub Actions · Jenkins · GitLab · Git  
**Application Platforms:** WildFly · Apache Tomcat · Java 21 · Maven  
**Databases:** PostgreSQL · MariaDB/MySQL · Oracle Database  
**Monitoring:** Centreon · Nagios · Prometheus · Grafana · NRPE · Node Exporter  
**Web & Hosting:** Nginx · Apache HTTP Server · ISPConfig · FTP · phpMyAdmin  
**Email Operations:** Postfix · Amavis · Rspamd · SpamAssassin · SPF · DKIM · DMARC · DNSBL/RBL checks  
**Infrastructure:** systemd · LVM · RAID · KVM · QEMU · Hyper-V · Docker  
**VMware:** vSphere (Linux VM operations, snapshots, test VM provisioning); ESXi events (read-only)  
**Networking:** TCP/IP · VLAN · routing · DNS · Cisco · firewalld · iptables  
**Tools:** SSH · curl · vim · Linux CLI

---

# 🚀 Featured Projects

## Ansible Infrastructure & CI/CD Lab

A practical infrastructure automation environment built around **Ansible, Linux, Java application servers, PostgreSQL and monitoring**.

The project is intentionally developed using fresh virtual machines to expose hidden assumptions and improve automation until infrastructure can be provisioned repeatedly and predictably.

### Current capabilities

- Debian and RHEL host bootstrap
- static IPv4, gateway and DNS configuration
- IPv6 policy automation
- privilege escalation managed with Ansible Vault
- WildFly provisioning
- Apache Tomcat 11 provisioning
- PostgreSQL provisioning
- Apache HTTP Server provisioning
- JDBC and JNDI datasource configuration
- declarative PostgreSQL `pg_hba.conf`
- application deployment verification
- SHA-256 artifact integrity checks
- deployment backup and rollback
- idempotency validation
- Nagios, Prometheus and Grafana onboarding
- Node Exporter and NRPE automation
- selective UTM VM startup and controlled lab shutdown
- one-command provisioning and deployment workflows

```text
Fresh Linux VM
      |
      v
 Host Bootstrap
      |
      +------------------+------------------+------------------+
      |                  |                  |                  |
      v                  v                  v                  v
   WildFly            Tomcat           PostgreSQL          Apache
      |                  |                  |                  |
      +-------- JDBC ----+----------------->|                  |
      |                                                        |
      +---------------- Monitoring -----------------------------+
                           |
                  +--------+--------+
                  |                 |
                  v                 v
               Nagios          Prometheus
                                   |
                                   v
                                 Grafana
```

### Main workflows

```bash
ansible-playbook bootstrap.yml --limit <host>

./deploy-lab.sh <wildfly-host>
./deploy-database.sh <database-host>
./deploy-apache.sh <apache-host>
./deploy-tomcat.sh <tomcat-host>

./start-lab.sh <host1> [host2 ...]
./halt-lab.sh
```

### Deployment and provisioning safeguards

- pre-flight validation before deployment
- remote database connectivity tests
- datasource verification
- WAR structure validation
- SHA-256 source/remote comparison
- build and deployment metadata
- automatic backup and rollback
- application endpoint verification
- repeated execution with `changed=0`

📦 **[Repository: ansible-lab](https://github.com/madamiuk/ansible-lab)**

---

## GitLab + Jenkins CI/CD Lab

A CI/CD environment built from scratch on **Debian 13**.

### Scope

- GitLab CE and Jenkins
- Nginx reverse proxy
- HTTPS and private CA
- GitLab private repository
- Protected Branch
- workflow: **feature branch → Merge Request → main**
- GitLab Webhook → Jenkins
- automated deployment to Nginx
- Project Access Token with minimal permissions
- troubleshooting of TLS, DNS, webhooks and services

```text
Developer
   |
   v
Feature Branch
   |
   v
Merge Request
   |
   v
Protected main
   |
   v
GitLab Webhook
   |
   v
Jenkins
   |
   v
Nginx
```

📦 **[Repository](https://github.com/madamiuk/gitlab-jenkins-cicd-lab)**  
📘 **[Technical documentation](https://madamiuk.github.io/gitlab-jenkins-cicd-lab/)**

---

# 💼 Experience

### Intratel Sp. z o.o. — Linux System Engineer (SUSE Linux Enterprise Server)
**12/2022 – 03/2025**

- Administered production and test Linux environments, particularly **SUSE Linux Enterprise Server**, and maintained infrastructure services supporting the company's cloud platform and external customers.
- Operated and troubleshot production **web, email, FTP and hosting services**, using tools including ISPConfig and phpMyAdmin.
- Maintained and secured **Postfix** email infrastructure with **Amavis, Rspamd and SpamAssassin**, including anti-spam rule analysis.
- Implemented and maintained **SPF, DKIM and DMARC**; investigated mail delivery issues, reviewed logs and checked mail server reputation and DNS-based blocklists.
- Monitored service availability using **Centreon**, diagnosed incidents and supported routine maintenance and system updates.
- Maintained OTP authentication systems based on **Yubico** keys, including database and validation servers.
- Used **VMware vSphere** to provision test VMs within assigned permissions, operate Linux VMs and take snapshots before OS upgrades and critical service changes.
- Reviewed **ESXi events with read-only access** during engineering on-call duties. VLAN assignment and VM network configuration were handled by the dedicated networking team; I did not administer ESXi hosts or VMware clusters.
- Worked with other infrastructure teams and maintained technical documentation.

### Areszt Śledczy w Hajnówce — IT Specialist / IT & Communications Team Coordinator
**11/2007 – 01/2022**

- Coordinated a four-person IT and communications team and supported the operation of server, networking, communications and security systems.
- Administered **Windows Server**, on-premises **Active Directory**, File Server, **Hyper-V** and Linux systems, including KVM/QEMU.
- Supported network and security infrastructure, CCTV, backups and storage systems including QNAP.
- Prepared technical specifications for public procurement and maintained hardware, software and license inventories.
- Documented systems and information security procedures.

### University Clinical Hospital, Medical University of Białystok — IT Specialist / Application Developer
**06/2005 – 10/2007**

- Developed and maintained internal hospital applications using **EJB, JSP, Apache Tomcat and Apache HTTP Server**.
- Implemented processes related to patient waiting lists and National Health Fund (NFZ) services.
- Produced and verified operational reports and analyses using **MySQL**.

### Centrum Nauki i Biznesu ŻAK — IT Instructor
**10/2005 – 06/2006 (overlapping appointment)**

- Taught operating systems, computer networks, structured and object-oriented programming, and computer hardware.

---

# 🎓 Education

**Białystok University of Technology**

- Computer Science — *Software Systems*
- Management Engineering — *Information Security Management*

---

# 📜 Certifications

- **SUSE Certified Engineer in SUSE Linux Enterprise Server 15**
- **SUSE Certified Administrator in SUSE Linux Enterprise Server 15**
- **CompTIA Security+ (SY0-701)**
- **Cisco Certified Network Associate (CCNA)**
- **Internal Auditor — ISO/IEC 27001 Information Security Management System**

---

# 🎯 Current focus

**Infrastructure Automation · Ansible · Terraform / OCI · CI/CD · Kubernetes · Observability · Python**

My primary professional background is **Linux systems and production infrastructure operations**. I continue to build practical labs in infrastructure automation, cloud provisioning and reproducible deployments.
