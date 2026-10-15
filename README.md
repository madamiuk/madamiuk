# 👨‍💻 Mirosław Adamiuk

📍 Straszewo, Polska  
📧 [miroslaw.adamiuk@gmail.com](mailto:miroslaw.adamiuk@gmail.com) | 💼 [LinkedIn](https://www.linkedin.com/in/miros%C5%82aw-adamiuk-548821222/) | 🌐 [GitHub](https://github.com/madamiuk)

---

## 🧾 Podsumowanie zawodowe

Administrator i inżynier systemów Linux z doświadczeniem w utrzymaniu środowisk produkcyjnych i testowych, zarządzaniu infrastrukturą IT oraz sieciami LAN/WAN.

Specjalizuję się w administracji systemami Linux, automatyzacji z wykorzystaniem **Ansible**, utrzymaniu usług i serwerów aplikacyjnych oraz monitoringu infrastruktury. Posiadam praktyczne doświadczenie w konfiguracji sieci, VLAN-ów, routingu oraz urządzeń Cisco.

Rozwijam kompetencje w kierunku **DevOps / Infrastructure Automation / Platform Engineering**, budując środowiska wykorzystujące Ansible, Git, GitHub Actions, Java Application Servers, PostgreSQL, Prometheus, Grafana, Nagios oraz automatyczne procesy CI/CD.

---

## 🛠️ Umiejętności techniczne

### Systemy operacyjne

Linux — SUSE Linux Enterprise Server, Red Hat Enterprise Linux, Oracle Linux, Debian  
Windows Server

### Automatyzacja i Infrastructure as Code

Ansible:

- inventories i grupowanie hostów
- playbooks i roles
- variables, defaults i precedence
- Jinja2 templates
- handlers
- facts i custom facts
- loops i conditionals
- `register`, `set_fact`, `assert`
- `block`, `rescue`, `always`
- delegation i `run_once`
- tags
- Ansible Vault
- privilege escalation
- idempotentna konfiguracja infrastruktury
- provisioning usług i aplikacji

### Monitoring i Observability

- Centreon
- Nagios Core
- NRPE
- Prometheus
- Node Exporter
- Grafana
- PromQL
- monitoring infrastruktury produkcyjnej
- monitoring hostów i usług
- monitoring CPU, RAM, load average, filesystem i sieci
- analiza alarmów i stanów usług
- provisioning dashboardów Grafana
- provisioning datasource Prometheus
- dynamiczne generowanie targetów Prometheus z inventory Ansible
- własne labels dla hostów
- własne pluginy/checki NRPE
- monitoring aplikacji i usług TCP/HTTP
- walidacja konfiguracji Prometheus przy użyciu `promtool`

### CI/CD i kontrola wersji

- Git
- GitHub
- GitHub Actions
- GitLab
- Jenkins
- CI/CD pipelines
- workflow automation
- build artifacts
- self-hosted runners
- automatyczny deployment aplikacji

### Konteneryzacja i wirtualizacja

- Docker
- KVM
- QEMU
- Hyper-V
- podstawy Kubernetes / Kind

### Java / Application Servers

- Java 21
- Maven
- Apache Tomcat 11
- WildFly 41
- deployment aplikacji WAR
- konfiguracja JDBC
- konfiguracja DataSource/JNDI

### Jakarta EE

- Jakarta REST
- EJB
- JPA
- DataSource / JNDI
- REST API

### Bazy danych

- PostgreSQL
- MariaDB / MySQL
- JDBC
- podstawy administracji Oracle Database

### Testowanie

- JUnit 5
- Mockito
- Maven Surefire
- testy jednostkowe
- testy integracyjne REST API

### Sieci

- LAN/WAN
- TCP/IP
- VLAN
- routing
- DNS
- podstawy bezpieczeństwa sieci
- diagnostyka połączeń i usług

### Urządzenia sieciowe

Cisco — konfiguracja i zarządzanie

### Usługi i serwery

- Apache HTTP Server
- Nginx
- WWW
- DNS
- poczta
- SSH
- PostgreSQL
- MariaDB
- Jenkins
- GitLab
- WildFly
- Tomcat

### Administracja Linux

- systemd
- LVM
- RAID
- zarządzanie pakietami
- użytkownicy i uprawnienia
- zarządzanie usługami
- analiza logów
- diagnostyka systemów
- firewalld
- iptables
- SSL/TLS
- troubleshooting

### Narzędzia

Linux CLI, Bash, SSH, Git, Ansible, Maven, curl, vim, PromQL

---

# 🚀 Projekty i laboratoria

## 🔧 Ansible Infrastructure & CI/CD Lab

Praktyczne laboratorium automatyzacji infrastruktury oraz wdrażania aplikacji z wykorzystaniem **Ansible, GitHub Actions, Java, WildFly i PostgreSQL**.

### Zrealizowane elementy

- budowa inventory Ansible z podziałem hostów według pełnionych ról
- tworzenie wielokrotnego użytku ról Ansible
- wykorzystanie variables, defaults, templates, handlers i facts
- testowanie variable precedence
- idempotentna konfiguracja serwerów
- automatyczna instalacja i konfiguracja Java 21
- automatyczna instalacja i konfiguracja Apache Tomcat 11
- automatyczna instalacja i konfiguracja WildFly 41
- zarządzanie usługami poprzez systemd
- wdrażanie aplikacji WAR za pomocą Ansible
- konfiguracja sterownika PostgreSQL JDBC
- konfiguracja DataSource/JNDI
- integracja aplikacji Jakarta EE z PostgreSQL
- implementacja REST API wykorzystującego EJB i JPA
- implementacja operacji CRUD na bazie PostgreSQL
- testy jednostkowe z wykorzystaniem JUnit 5 i Mockito
- testy integracyjne REST API
- budowanie aplikacji przy użyciu Maven
- tworzenie pipeline'u CI w GitHub Actions
- automatyczne wykonywanie testów i budowanie WAR
- publikowanie WAR jako GitHub Actions Artifact
- konfiguracja self-hosted GitHub Actions Runner na macOS ARM64
- automatyczny deployment aplikacji poprzez Ansible
- automatyczne uruchamianie CD po pomyślnym zakończeniu CI
- powiązanie deploymentu z artefaktem wygenerowanym przez konkretny przebieg CI
- weryfikacja wdrożonej aplikacji poprzez HTTP/REST
- zachowanie ręcznego deploymentu jako mechanizmu awaryjnego

### 🔄 Zbudowany pipeline CI/CD

```text
Git Push
   │
   ▼
GitHub Actions CI
   │
   ├── Java 21
   ├── Maven
   ├── Unit Tests
   ├── Integration Tests
   └── WAR Build
          │
          ▼
     WAR Artifact
          │
          ▼
   Successful CI
          │
          ▼
GitHub Actions CD
          │
          ▼
Self-hosted Runner
     macOS ARM64
          │
          ▼
       Ansible
          │
          ▼
      Debian Linux
          │
          ▼
       WildFly
          │
          ▼
   Jakarta EE REST API
          │
          ▼
      PostgreSQL
          │
          ▼
     HTTP Verification
```

---

## 📊 Monitoring & Observability Lab

Rozbudowa laboratorium Ansible o kompletny stos monitoringu infrastruktury Linux.

Doświadczenie laboratoryjne uzupełnia praktyka zawodowa z **Centreon**, wykorzystywanym do monitoringu infrastruktury podczas pracy w Intratel Sp. z o.o.

### Architektura

```text
                    Ansible
                       │
        ┌──────────────┼──────────────┐
        │              │              │
        ▼              ▼              ▼
   Nagios Core     Prometheus       Grafana
        │              │              │
        ▼              ▼              │
       NRPE       Node Exporter        │
        │              │              │
        └──── Linux Hosts ─────────────┘
```

### Centreon

Praktyczne doświadczenie zawodowe:

- monitoring infrastruktury i usług
- analiza statusów hostów i usług
- obsługa alarmów i zdarzeń
- identyfikacja problemów z dostępnością usług
- wsparcie diagnostyki incydentów infrastrukturalnych
- bieżąca obserwacja kondycji środowisk Linux

### Nagios Core

- automatyczna instalacja i konfiguracja Nagios Core przez Ansible
- generowanie konfiguracji hostów na podstawie inventory
- dynamiczne generowanie usług monitorowanych przez Nagios
- monitoring hostów Linux
- monitoring usług HTTP
- walidacja konfiguracji Nagios
- centralizacja monitoringu na dedykowanym serwerze

### NRPE

- instalacja i konfiguracja NRPE na Debian i RHEL
- obsługa różnych ścieżek pluginów zależnie od dystrybucji
- ograniczenie dostępu do NRPE wyłącznie do serwera monitorującego
- konfiguracja firewalld
- monitoring WildFly przez lokalny test TCP
- monitoring system load
- monitoring filesystem `/`
- monitoring liczby procesów
- własny plugin Bash do monitorowania pamięci RAM
- integracja własnych checków z Nagios

### Prometheus

- automatyczna instalacja Prometheus przez Ansible
- dynamiczne generowanie scrape targets na podstawie inventory
- konfiguracja Node Exporter na wszystkich hostach
- automatyczne wykrywanie architektury ARM64 / AMD64
- konfiguracja systemd
- ograniczenie dostępu do portu Node Exporter przy użyciu firewalld
- własne labels identyfikujące hosty
- walidacja konfiguracji przez `promtool`
- monitoring wszystkich targetów przez Prometheus API
- zbieranie metryk w interwale 15 sekund

### Grafana

- automatyczna instalacja Grafana przez Ansible
- provisioning datasource Prometheus
- provisioning dashboardów z pliku JSON
- dostęp do Grafana przez tunel SSH
- dynamiczny wybór hosta z poziomu dashboardu
- wykorzystanie własnego labela `host`
- PromQL wykorzystujący selekcję hostów
- automatyczne aktualizowanie dashboardów przez Ansible

### Dashboard infrastruktury

Dashboard obejmuje:

- CPU usage
- Memory usage
- Load 1 min
- Load 5 min
- Load 15 min
- Network receive
- Network transmit
- Root filesystem usage

Monitoring obejmuje hosty:

```text
oracle01
oracle02
debian01
debian02
rhel01
database01
```

### Przykładowy przepływ metryk

```text
Linux Host
   │
   ▼
Node Exporter
   │
   ▼
Prometheus
   │
   ▼
PromQL
   │
   ▼
Grafana Dashboard
```

### Podejście do monitoringu

```text
Centreon
    │
    └── praktyczny monitoring infrastruktury w środowisku zawodowym

Nagios + NRPE
    │
    └── alerting, dostępność usług, lokalne checki

Prometheus + Node Exporter
    │
    └── metryki i dane historyczne

Grafana
    │
    └── wizualizacja i dashboardy
```

Cała konfiguracja laboratoryjnego stosu monitoringu jest zarządzana jako kod przy użyciu Ansible.

---

## 🔧 GitLab + Jenkins CI/CD Lab

Praktyczne laboratorium CI/CD zbudowane od podstaw na **Debian 13**, obejmujące pełny workflow od pracy developera do automatycznego wdrożenia aplikacji.

**Technologie:** Debian Linux · GitLab CE · Jenkins · Nginx · Git · OpenJDK · Bash · TLS/PKI

### Zakres projektu

- instalacja i konfiguracja GitLab CE oraz Jenkins
- Nginx jako reverse proxy dla GitLab i Jenkins
- HTTPS z własnym CA i certyfikatami TLS
- prywatne repozytorium GitLab i kontrola dostępu
- Jenkins deployment do `/var/www`
- automatyczny pipeline **GitLab Webhook → Jenkins → Nginx**
- Protected Branch
- workflow **feature branch → Merge Request → main**
- Project Access Token zgodny z zasadą minimalnych uprawnień
- diagnostyka DNS, portów, TLS, webhooków i GitLab outbound requests
- audyt usług i portów środowiska

```text
Developer
    │
    ▼
Feature Branch
    │
    ▼
GitLab
    │
    ▼
Merge Request
    │
    ▼
Protected main
    │
    ▼
HTTPS Webhook
    │
    ▼
Jenkins
    │
    ▼
/var/www/web-demo
    │
    ▼
Nginx
```

📦 **[Repozytorium projektu](https://github.com/madamiuk/gitlab-jenkins-cicd-lab)**  
📘 **[Pełna dokumentacja techniczna](https://madamiuk.github.io/gitlab-jenkins-cicd-lab/)**

---

# 💼 Doświadczenie zawodowe

## 🏢 Intratel Sp. z o.o. — *Inżynier Systemowy*

📅 12/2022 – 03/2025

- Administrowanie systemami Linux w środowiskach produkcyjnych i testowych
- Konfiguracja i utrzymanie sieci LAN/WAN
- Monitoring infrastruktury i usług z wykorzystaniem **Centreon**
- Analiza alarmów, stanów hostów i usług oraz wsparcie diagnostyki incydentów
- Reagowanie na incydenty i awarie infrastruktury IT
- Współpraca z zespołami developerskimi przy wdrażaniu i utrzymaniu aplikacji
- Tworzenie i aktualizacja dokumentacji technicznej

## 🏢 Areszt Śledczy w Hajnówce — *Specjalista ds. Informatyki*

📅 11/2007 – 01/2022

- Koordynacja czteroosobowego zespołu ds. informatyki i łączności
- Odpowiedzialność za infrastrukturę IT, łączność przewodową i bezprzewodową, zabezpieczenia elektroniczne oraz monitoring CCTV
- Administracja lokalnymi systemami informatycznymi
- Instalacja, konfiguracja i zarządzanie Windows Server 2016 — Hyper-V, File Server, Active Directory
- Administracja systemami Linux — DHCP, Samba, KVM, QEMU, MySQL, Squid
- Zarządzanie systemami QNAP i rozwiązaniami backupowymi
- Pełnienie funkcji inspektora bezpieczeństwa teleinformatycznego zgodnie z ustawą o ochronie informacji niejawnych
- Opracowywanie i wdrażanie dokumentacji bezpieczeństwa systemów teleinformatycznych

---

# 🎓 Wykształcenie

🎓 **Politechnika Białostocka**  
*Inżynieria zarządzania — Zarządzanie bezpieczeństwem informacji*  
📅 2018

🎓 **Politechnika Białostocka**  
*Informatyka — Systemy oprogramowania*  
📅 2000 – 2007

---

# 📜 Certyfikaty

- 🏅 Cisco Certified Network Associate (CCNA) — 2003
- 🏅 Auditor wewnętrzny SZBI PN-EN ISO/IEC 27001 — 2017
- 🏅 SUSE Certified Engineer in SUSE Linux Enterprise Server 15 — 2023
- 🏅 SUSE Certified Administrator in SUSE Linux Enterprise Server 15 — 2023
- 🏅 CompTIA Security+ (SY0-701) — 2024

---

# 🌍 Języki

- 🇵🇱 Polski — ojczysty
- 🇬🇧 Angielski — B2

---

# 📊 GitHub Stats

![GitHub stats](https://github-stats-extended.vercel.app/api?username=madamiuk&show_icons=true&theme=default)

---

# 📌 Obecny kierunek rozwoju

Aktualnie rozwijam kompetencje w obszarach:

- Infrastructure as Code
- zaawansowana automatyzacja Ansible
- CI/CD i GitHub Actions
- administracja i automatyzacja środowisk Linux
- monitoring i observability
- Prometheus i PromQL
- Grafana i dashboard provisioning
- alerting i monitoring usług
- konteneryzacja i orkiestracja
- Kubernetes
- Java Application Servers
- DevOps / Platform Engineering
- Python jako narzędzie automatyzacji infrastruktury

---

# 📌 Dodatkowe informacje

- Gotowość do pracy w modelu hybrydowym / zdalnym
- Zainteresowania: starożytne cywilizacje, literatura fantastyczna, fizyka kwantowa

---

*⭐ Dziękuję za odwiedzenie mojego profilu!*
