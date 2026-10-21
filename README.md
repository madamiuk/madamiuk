# 👨‍💻 Mirosław Adamiuk

**Linux System Engineer · DevOps · Infrastructure Automation**

📍 Polska  
📧 [miroslaw.adamiuk@gmail.com](mailto:miroslaw.adamiuk@gmail.com) · 💼 [LinkedIn](https://www.linkedin.com/in/miros%C5%82aw-adamiuk-548821222/) · 🌐 [GitHub](https://github.com/madamiuk)

---

## 👋 O mnie

Inżynier systemów Linux z doświadczeniem w administracji środowiskami produkcyjnymi i testowymi, infrastrukturą IT, sieciami oraz monitoringiem.

Specjalizuję się w systemach Linux i automatyzacji infrastruktury z wykorzystaniem **Ansible**. Rozwijam kompetencje w kierunku **DevOps, Infrastructure Automation i Platform Engineering**, budując praktyczne laboratoria obejmujące CI/CD, application servers, monitoring oraz automatyczne wdrożenia.

Interesuje mnie przede wszystkim tworzenie środowisk, które są **powtarzalne, mierzalne, łatwe do wdrożenia i możliwe do odtworzenia jako kod**.

---

# 🛠️ Tech Stack

**Linux:** SUSE Linux Enterprise Server · RHEL · Oracle Linux · Debian  
**Automation:** Ansible · Bash · Jinja2 · Ansible Vault  
**CI/CD:** GitHub Actions · Jenkins · GitLab · Git  
**Application Servers:** WildFly · Apache Tomcat  
**Monitoring:** Centreon · Nagios · Prometheus · Grafana · NRPE · Node Exporter  
**Databases:** PostgreSQL · MariaDB/MySQL · Oracle Database  
**Web:** Nginx · Apache HTTP Server  
**Java:** Java 21 · Maven · Jakarta EE · JPA · EJB · REST  
**Infrastructure:** systemd · LVM · RAID · KVM · QEMU · Docker  
**Networking:** TCP/IP · VLAN · routing · DNS · Cisco · firewalld · iptables  
**Tools:** SSH · curl · vim · PromQL · Linux CLI

---

# 🚀 Projekty

## 🔧 Ansible Infrastructure & CI/CD Lab

Praktyczne środowisko automatyzacji deploymentu aplikacji **Java / WildFly / PostgreSQL** zarządzane przez Ansible i GitHub Actions.

### Najważniejsze elementy

- role Ansible dla WildFly i PostgreSQL
- idempotentna konfiguracja infrastruktury
- automatyczny build WAR w GitHub Actions
- self-hosted GitHub Actions Runner na macOS ARM64
- pipeline **GitHub Actions → Ansible → WildFly**
- PostgreSQL JDBC oraz DataSource/JNDI
- pre-flight validation przed deploymentem
- SHA-256 artefaktu i weryfikacja integralności
- Git commit SHA oraz build metadata zapisane w WAR
- automatyczny backup i rollback
- rotacja backupów WAR
- weryfikacja REST endpointu po wdrożeniu
- końcowy raport deploymentu zawierający wersję, commit i checksumę

```text
Git Push
   │
   ▼
GitHub Actions CI
   │
   ▼
WAR Artifact
   │
   ▼
GitHub Actions CD
   │
   ▼
Self-hosted Runner
   │
   ▼
Ansible
   │
   ▼
WildFly ─────► PostgreSQL
   │
   ├── pre-flight validation
   ├── SHA-256 verification
   ├── deployment
   ├── automatic rollback
   └── REST verification
```

📦 **[Repozytorium: ansible-lab](https://github.com/madamiuk/ansible-lab)**

---

## 📊 Monitoring & Observability Lab

Laboratorium monitoringu infrastruktury Linux zarządzane jako kod przy użyciu Ansible.

### Stack

**Nagios Core · NRPE · Prometheus · Node Exporter · Grafana · PromQL**

### Zakres

- automatyczna instalacja i konfiguracja monitoringu
- dynamiczne generowanie hostów i usług z inventory Ansible
- monitoring CPU, RAM, load, filesystem i sieci
- własne checki NRPE
- monitoring usług HTTP/TCP
- provisioning Prometheus i Grafana
- automatyczne dashboardy
- obsługa architektur ARM64 i AMD64
- walidacja konfiguracji Prometheus przez `promtool`

```text
Linux Hosts
   │
   ├── NRPE ─────► Nagios
   │
   └── Node Exporter
            │
            ▼
        Prometheus
            │
            ▼
         Grafana
```

Doświadczenie laboratoryjne uzupełnia praktyka zawodowa z systemem **Centreon**.

---

## 🔧 GitLab + Jenkins CI/CD Lab

Laboratorium CI/CD zbudowane od podstaw na **Debian 13**.

### Zakres

- GitLab CE oraz Jenkins
- Nginx jako reverse proxy
- HTTPS i własne CA
- prywatne repozytorium GitLab
- Protected Branch
- workflow **feature branch → Merge Request → main**
- GitLab Webhook → Jenkins
- automatyczny deployment do Nginx
- Project Access Token zgodny z zasadą minimalnych uprawnień
- diagnostyka TLS, DNS, webhooków i usług

```text
Developer
   │
   ▼
Feature Branch
   │
   ▼
Merge Request
   │
   ▼
Protected main
   │
   ▼
GitLab Webhook
   │
   ▼
Jenkins
   │
   ▼
Nginx
```

📦 **[Repozytorium projektu](https://github.com/madamiuk/gitlab-jenkins-cicd-lab)**  
📘 **[Dokumentacja techniczna](https://madamiuk.github.io/gitlab-jenkins-cicd-lab/)**

---

# 💼 Doświadczenie

### Intratel Sp. z o.o. — Inżynier Systemowy
**12/2022 – 03/2025**

- administracja systemami Linux
- utrzymanie środowisk produkcyjnych i testowych
- sieci LAN/WAN
- monitoring infrastruktury z wykorzystaniem Centreon
- analiza incydentów i problemów z dostępnością usług
- współpraca przy wdrażaniu i utrzymaniu aplikacji
- dokumentacja techniczna

### Areszt Śledczy w Hajnówce — Specjalista ds. Informatyki
**11/2007 – 01/2022**

- koordynacja zespołu IT i łączności
- administracja Windows Server i Linux
- Active Directory · Hyper-V · KVM · QEMU
- infrastruktura sieciowa i systemy bezpieczeństwa
- QNAP i rozwiązania backupowe
- bezpieczeństwo teleinformatyczne
- dokumentacja bezpieczeństwa systemów IT

---

# 🎓 Wykształcenie

**Politechnika Białostocka**  
🎓 Informatyka — *Systemy oprogramowania*  
🎓 Inżynieria zarządzania — *Zarządzanie bezpieczeństwem informacji*

---

# 📜 Certyfikaty

- **SUSE Certified Engineer in SUSE Linux Enterprise Server 15**
- **SUSE Certified Administrator in SUSE Linux Enterprise Server 15**
- **CompTIA Security+ (SY0-701)**
- **Cisco Certified Network Associate (CCNA)**
- **Auditor wewnętrzny SZBI PN-EN ISO/IEC 27001**

---

# 🎯 Obecny kierunek rozwoju

**DevOps · Infrastructure as Code · Platform Engineering · CI/CD · Kubernetes · Observability · Python Automation**

Aktualnie rozwijam się przede wszystkim w kierunku automatyzacji infrastruktury i procesów deploymentu oraz budowania środowisk zarządzanych jako kod.

---

# 🌍 Języki

🇵🇱 Polski — ojczysty  
🇬🇧 Angielski — B2

---

# 📊 GitHub Stats

![GitHub stats](https://github-stats-extended.vercel.app/api?username=madamiuk&show_icons=true&theme=default)

---

⭐ *Dziękuję za odwiedzenie mojego profilu.*
