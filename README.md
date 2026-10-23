# 👨‍💻 Mirosław Adamiuk

**Linux System Engineer | Infrastructure Automation | DevOps**

📍 Poland  
💼 [LinkedIn](https://www.linkedin.com/in/miros%C5%82aw-adamiuk-548821222/) · 🌐 [GitHub](https://github.com/madamiuk)

---

## About me

Linux System Engineer with hands-on experience in Linux infrastructure, networking, monitoring, production support and troubleshooting.

I focus on building repeatable infrastructure workflows with **Ansible, Bash and Git**, covering fresh-host bootstrap, service provisioning, application deployment, database connectivity, CI/CD and observability.

My current direction is **DevOps, Infrastructure as Code and Platform Engineering**, with a strong focus on practical automation and reproducible environments.

---

## ⚡ Highlights

- Linux administration in production and test environments
- Infrastructure automation with **Ansible**
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
**Web:** Nginx · Apache HTTP Server  
**Infrastructure:** systemd · LVM · RAID · KVM · QEMU · Docker  
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

### Intratel Sp. z o.o. — System Engineer
**12/2022 – 03/2025**

- Linux infrastructure administration
- production and test environment support
- LAN/WAN networking
- infrastructure monitoring with Centreon
- service availability and incident troubleshooting
- application and infrastructure maintenance
- technical documentation

### Areszt Śledczy w Hajnówce — IT Specialist
**11/2007 – 01/2022**

- IT and communications team coordination
- Windows Server and Linux administration
- Active Directory, Hyper-V, KVM and QEMU
- networking and security infrastructure
- backup and storage systems
- information security documentation

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

**DevOps · Infrastructure as Code · Platform Engineering · CI/CD · Kubernetes · Observability · Python Automation**

I am currently developing further in infrastructure automation, repeatable deployment workflows and platform-oriented engineering practices.
