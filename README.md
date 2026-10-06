# 👨‍💻 Mirosław Adamiuk

📍 Straszewo, Polska
📧 [miroslaw.adamiuk@gmail.com](mailto:miroslaw.adamiuk@gmail.com) | 💼 [LinkedIn](https://www.linkedin.com/in/miros%C5%82aw-adamiuk-548821222/) | 🌐 [GitHub](https://github.com/madamiuk)

---

## 🧾 Podsumowanie zawodowe

Administrator i inżynier systemów Linux z doświadczeniem w utrzymaniu środowisk produkcyjnych i testowych, zarządzaniu infrastrukturą IT oraz sieciami LAN/WAN.

Specjalizuję się w administracji systemami Linux, automatyzacji z wykorzystaniem Ansible oraz utrzymaniu usług i serwerów aplikacyjnych. Posiadam praktyczne doświadczenie w konfiguracji sieci, VLAN-ów, routingu oraz urządzeń Cisco.

Rozwijam kompetencje w kierunku **DevOps / Infrastructure Automation**, budując środowiska wykorzystujące Ansible, Git, GitHub Actions, Java Application Servers, PostgreSQL oraz automatyczne procesy CI/CD.

---

## 🛠️ Umiejętności techniczne

**Systemy operacyjne:**
Linux — SUSE Linux Enterprise Server, Red Hat / Oracle Linux, Debian
Windows Server

**Automatyzacja i Infrastructure as Code:**
Ansible — inventories, playbooks, roles, variables, templates, handlers, facts, privilege escalation, idempotent configuration

**CI/CD i kontrola wersji:**
Git, GitHub, GitHub Actions, CI/CD pipelines, workflow automation, build artifacts, self-hosted runners

**Konteneryzacja i wirtualizacja:**
Docker, KVM, QEMU, Hyper-V

**Java / Application Servers:**
Java 21, Maven, Apache Tomcat 11, WildFly 41, deployment aplikacji WAR

**Jakarta EE:**
Jakarta REST, EJB, JPA, DataSource/JNDI

**Bazy danych:**
PostgreSQL, MariaDB/MySQL, JDBC

**Testowanie:**
JUnit 5, Mockito, Maven Surefire, testy jednostkowe i integracyjne REST API

**Sieci:**
LAN/WAN, TCP/IP, VLAN, routing, podstawy bezpieczeństwa sieci

**Urządzenia sieciowe:**
Cisco — konfiguracja i zarządzanie

**Usługi i serwery:**
Apache HTTP Server, WWW, DNS, poczta, SSH, bazy danych

**Administracja Linux:**
systemd, LVM, RAID, zarządzanie pakietami, użytkownikami, usługami, logami i diagnostyka systemów

**Narzędzia:**
Linux CLI, Bash, SSH, Git, Ansible, Maven, curl

---

## 🚀 Projekty i laboratoria

### 🔧 Ansible Infrastructure & CI/CD Lab

Praktyczne laboratorium automatyzacji infrastruktury oraz wdrażania aplikacji z wykorzystaniem **Ansible, GitHub Actions, Java, WildFly i PostgreSQL**.

### Zrealizowane elementy

* budowa inventory Ansible z podziałem hostów według pełnionych ról
* tworzenie wielokrotnego użytku ról Ansible
* wykorzystanie variables, defaults, templates, handlers i facts
* idempotentna konfiguracja serwerów
* automatyczna instalacja i konfiguracja Java 21
* automatyczna instalacja i konfiguracja Apache Tomcat 11
* automatyczna instalacja i konfiguracja WildFly 41
* zarządzanie usługami poprzez systemd
* wdrażanie aplikacji WAR za pomocą Ansible
* konfiguracja sterownika PostgreSQL JDBC
* konfiguracja DataSource/JNDI
* integracja aplikacji Jakarta EE z PostgreSQL
* implementacja REST API wykorzystującego EJB i JPA
* implementacja operacji CRUD na bazie PostgreSQL
* testy jednostkowe z wykorzystaniem JUnit 5 i Mockito
* testy integracyjne REST API
* budowanie aplikacji przy użyciu Maven
* tworzenie pipeline'u CI w GitHub Actions
* automatyczne wykonywanie testów i budowanie WAR
* publikowanie WAR jako GitHub Actions Artifact
* konfiguracja self-hosted GitHub Actions Runner na macOS ARM64
* uruchamianie self-hosted runnera jako usługi systemowej macOS
* automatyczny deployment aplikacji poprzez Ansible
* automatyczne uruchamianie CD po pomyślnym zakończeniu CI
* powiązanie deploymentu z artefaktem wygenerowanym przez konkretny przebieg CI
* weryfikacja wdrożonej aplikacji poprzez HTTP/REST
* zachowanie ręcznego deploymentu jako mechanizmu awaryjnego

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

## 💼 Doświadczenie zawodowe

### 🏢 Intratel Sp. z o.o. — *Inżynier Systemowy*

📅 12/2022 – 03/2025

* Administrowanie systemami Linux w środowiskach produkcyjnych i testowych
* Konfiguracja i utrzymanie sieci LAN/WAN
* Monitorowanie infrastruktury IT oraz reagowanie na incydenty i awarie
* Współpraca z zespołami developerskimi przy wdrażaniu i utrzymaniu aplikacji
* Tworzenie i aktualizacja dokumentacji technicznej

### 🏢 Areszt Śledczy w Hajnówce — *Specjalista ds. Informatyki*

📅 11/2007 – 01/2022

* Koordynacja czteroosobowego zespołu ds. informatyki i łączności
* Odpowiedzialność za infrastrukturę IT, łączność przewodową i bezprzewodową, zabezpieczenia elektroniczne oraz monitoring CCTV
* Administracja lokalnymi systemami informatycznymi
* Instalacja, konfiguracja i zarządzanie Windows Server 2016 — Hyper-V, File Server, Active Directory
* Administracja systemami Linux — DHCP, Samba, KVM, QEMU, MySQL, Squid
* Zarządzanie systemami QNAP i rozwiązaniami backupowymi
* Pełnienie funkcji inspektora bezpieczeństwa teleinformatycznego zgodnie z ustawą o ochronie informacji niejawnych
* Opracowywanie i wdrażanie dokumentacji bezpieczeństwa systemów teleinformatycznych

---

## 🎓 Wykształcenie

🎓 **Politechnika Białostocka**
*Inżynieria zarządzania — Zarządzanie bezpieczeństwem informacji*
📅 2018

🎓 **Politechnika Białostocka**
*Informatyka — Systemy oprogramowania*
📅 2000 – 2007

---

## 📜 Certyfikaty

* 🏅 Cisco Certified Network Associate (CCNA) — 2003
* 🏅 Auditor wewnętrzny SZBI PN-EN ISO/IEC 27001 — 2017
* 🏅 SUSE Certified Engineer in SUSE Linux Enterprise Server 15 — 2023
* 🏅 SUSE Certified Administrator in SUSE Linux Enterprise Server 15 — 2023
* 🏅 CompTIA Security+ (SY0-701) — 2024

---

## 🌍 Języki

* 🇵🇱 Polski — ojczysty
* 🇬🇧 Angielski — B2

---

## 📊 GitHub Stats

![GitHub stats](https://github-stats-extended.vercel.app/api?username=madamiuk\&show_icons=true\&theme=default)

---

## 📌 Obecny kierunek rozwoju

Rozwijam kompetencje w obszarach:

* Infrastructure as Code i automatyzacja infrastruktury
* Ansible
* CI/CD i GitHub Actions
* administracja i automatyzacja środowisk Linux
* konteneryzacja i orkiestracja
* Java Application Servers
* monitoring i observability
* DevOps / Platform Engineering

---

## 📌 Dodatkowe informacje

* Gotowość do pracy w modelu hybrydowym / zdalnym
* Zainteresowania: starożytne cywilizacje, literatura fantastyczna, fizyka kwantowa

---

*⭐ Dziękuję za odwiedzenie mojego profilu!*
