# LE XUAN NHI

**Current Position:** Tech Lead  
**Date of Birth:** Sep 10, 1991  
**Gender:** Male  

---

## Summary

10+ years of software engineering experience, transitioning from Java backend development into DevOps and Cloud Infrastructure. Joining projects end to end — analyze requirements, define scope, estimate realistically, plan and execute, manage status/risks, and handle deployment, turning client needs into reliable, prod-ready solutions. Specialized in designing, building, and operating systems on AWS and Kubernetes — with a strong focus on blockchain-related platforms, trading systems, and payment gateways (fintech).

- **Cloud Infrastructure:** Design and implement scalable, highly available AWS architectures following Well-Architected Framework principles.
- **Kubernetes & Containers:** Deploy and operate production Kubernetes clusters; manage CI/CD pipelines, GitOps workflows, and container-based services.
- **Blockchain Systems:** Build and operate RPC node infrastructure, validator monitoring, and Web3 platform services.
- **Security & Compliance:** Maintain PCI DSS-compliant environments, investigate security issues, and recommend fixes.
- **Tech Lead:** Guide team members, review code, and work directly with clients to clarify requirements and deliver solutions.
- **Problem Solving:** Strong root-cause analysis skills — able to investigate live issues across infrastructure, application, and network layers.
- **Project Management:** Define scope, break down tasks, estimate effort, track progress, manage risks, and coordinate across team members to keep projects on schedule and within quality standards.

---

## Technical Skills

| Domain | Capability | Key Technologies |
|---|---|---|
| **Cloud & Infrastructure** | Design, deploy, and operate scalable cloud environments; | AWS (EC2/ECS, VPC, RDS, S3, Lambda, WAF...), Terraform, Ansible, Linux |
| **Containers & k8s** | Set up and manage k8s clusters; handle networking, routing, and storage | k8s, Docker, Helm, Traefik, Cilium, KCL, Rancher |
| **Backend Development** | Build server-side applications, REST APIs, and microservices | Java, Spring Boot, Spring Cloud, JavaScript/TypeScript, NodeJS, NestJS |
| **Databases & Messaging** | Store and manage data; handle async communication and service coordination | MySQL/PostgreSQL, Oracle, MongoDB, Redis, RocketMQ, Zookeeper, Consul |
| **DevOps & CI/CD** | Automate build, test and deployment pipelines; maintain system observability and reliability | GitHub Actions, Jenkins, ArgoCD, GitOps, Prometheus, Grafana, Loki, ELK Stack |
| **Security & Compliance** | Harden infrastructure, maintain compliance standards, investigate and remediate issues | PCI DSS, Keycloak, OAuth2 Proxy, cert-manager, Sealed Secrets, WAF |
| **System Design & Architecture** | Design scalable, highly available architectures; define service boundaries, data flows, and infrastructure blueprints | Microservices, AWS Well-Architected Framework, Blockchain infrastructure |
| **Management** | Lead teams, manage scope and timeline, conduct code reviews, communicate directly with clients | Scrum, technical documentation, mentoring, risk management |

---

## Language Skills

- **English:** Intermediate

---

## Education

**2010-2012** — Programmer Course, Softech Aptech International Programmer Training Center in Da Nang

---

## Projects

### k8s Infrastructure Migration – Ingress to Gateway API

**Position: DevOps Engineer**  
**Duration: 10/2025 - now**  
**Team size: 4 people**  


**Description:**
An OSS infrastructure maintenance initiative on a production Kubernetes cluster (v1.32, 4 nodes, Cilium CNI). Migrated the L7 routing layer from Ingress NGINX to Traefik Gateway API ahead of NGINX Ingress end-of-support (March 2026).

**Responsibilities:**
- Reviewed 8 Gateway API implementations and recommended Traefik based on dual-mode support and low migration complexity.
- Wrote the Migration Design Document covering architecture decisions, TLS strategy, and rollback plan.
- Set up zero-downtime migration using blue-green DNS switching, allowing services to be cut over one by one.
- Replaced per-service TLS certificates with a single multi-SAN certificate managed by cert-manager.
- Configured Traefik for advanced use cases: OAuth2 auth, Basic Auth, Sticky Sessions, and HTTPS backends.
- Migrated 11 production services to Gateway API (all verified): Alertmanager, Prometheus, Grafana, Loki, Kubernetes Dashboard, OpenUnison, ArgoCD, Harbor, and others.
- Updated Cilium Network Policies and maintained full GitOps workflow via ArgoCD throughout.

**Technologies:**
- Kubernetes, Traefik, Kubernetes Gateway API (HTTPRoute / GatewayClass / Gateway), cert-manager, Let's Encrypt, Cilium, ArgoCD, KCL, Helm, Prometheus, Grafana, Keycloak, OAuth2 Proxy, Sealed Secrets

---

### Payment Gateway Platform

**Position: DevOps Engineer**  
**Duration: 8/2025 - now**  
**Team size: 3 people**  


**Description:**
A payment gateway platform supporting credit/debit card processing and digital wallet integration (Google Pay, Apple Pay), deployed on AWS with PCI DSS compliance requirements.

**Responsibilities:**
- Maintained and operated the production AWS environment, ensuring system stability and PCI DSS compliance.
- Built cost-optimized Sandbox environments as an alternative to production-equivalent environments, reducing cloud costs while keeping them fully usable.
- Designed and implemented CI/CD pipelines with GitHub Actions for all environments (sandbox, staging, production).
- Checked production systems against PCI DSS standards; found issues and gave recommendations to fix them.
- Helped the development team investigate application logs and handled direct actions to support end-users during incidents.

**Technologies:**
- AWS (EC2, RDS, S3, WAF, ALB), Kubernetes, Docker, GitHub Actions, NGINX, MySQL, Redis, Prometheus, Grafana, cert-manager, PCI DSS

---

### Blockchain Validator Monitoring System

**Position: TechLead**  
**Duration: 11/2025 - now**  
**Team size: 4 people**  


**Description:**
A centralized system to monitor multiple blockchain validators: software version, hardware metrics, node health check, status,...

**Responsibilities:**
- Participated in system architecture design; defined service boundaries and data flow for metrics pipeline
- Conducted code reviews for backend services
- Built a metrics collector service in NestJS.
- Streamed metrics to S3.
- Implemented real-time alerts using Redis Pub/Sub.
- Technologies: ReactJS, NestJS, Redis, Docker, Bash Script, AWS.

---

### Blockchain RPC Node System

**Position: TechLead**  
**Duration: 06/2025 - 10/2025**  
**Team size: 6 people**  


**Description:**
Challeng with request high scalability and throughput

**Responsibilities:**
- Lead of design and develop the ETH and BTC RPC node to running in B2B side.
- Implement health check solution for Node
- Designed AWS infrastructure for high availability and scalability; documented architecture decisions
- Setup AWS Infrastructure based on design
- Technologies: Javascript, Typescript, AWS, Terraform

---

### Blockchain RPC Provider

**Position: Infrastructure Engineer**  
**Team size: 5 members**  
**Duration: 04/2024 - 03/2025**  


**Description:**
A reliable and scalable RPC platform providing seamless access to multiple blockchain networks. Built on Kubernetes (K8s) for enhanced scalability, resilience, and efficient resource management, it ensures high-performance connectivity, real-time data retrieval, and secure infrastructure for building and scaling decentralized applications (dApps) across diverse blockchain ecosystems.

**Responsibilities:**
- Analyze client’s requirements.
- Design Infrastructure architecture solutions that align with requirements are scalable, high available, and secure.
- Deploy infrastructure using Infrastructure as Code (IaC) tools using Terraform and Ansible.
- Implement and optimize CI/CD pipelines for efficient application deployment.
- Implement monitoring solutions to track performance, availability, logs.
- Collaborate with customers and other members to identify and resolve infrastructure problems.

**Technologies:**
- Terraform, Ansible,
- Kubernetes (K8s) from scratch
  - High available with 3 Master Nodes.
  - Register Worker Node to Master Node using Bootstrap Tokens.
  - Using Nginx Service, Load Balancer and Ingress for routing requests based on domain.
  - Config firewall, traffic inbound, outbound between services from scratch.
  - Mount external disk as a volume for data storing.
  - Setup Rancher - a platform that allows delivering Kubernetes-as-a-Service
  - Setup Grafana, Loki, Prometheus to monitor system.
  - Built on Sakura Cloud - a service that owned by Sakura Internet from Japan

---

### Web3 Ecosystem Platform

**Position: Infrastructure Engineer (Team Leader)**  
**Team size: 130 members**  
**Duration: 10/2022 - 08/2024**  


**Description:**
Build a Web3 ecosystem integrating a crypto wallet, marketplace, and blockchain-based services for seamless user interaction with decentralized technology.
The wallet enables secure asset management, transactions, and interaction with dApps. The marketplace allows users to trade digital assets, NFTs, and services with smart contract automation.

**Responsibilities:**
- Designing AWS infrastructure architecture solutions that align with requirements and are scalable, highly available, and secure.
- Implementing and managing AWS services, including computing, storage, databases, networking, and security.
- Deploying infrastructure using Infrastructure as Code (IaC) tools using AWS CloudFormation
- Implementing and optimizing CI/CD pipelines for efficient application deployment.
- Implementing monitoring solutions to track performance, availability, and cost.
- Collaborating with other teams to identify and resolve complex infrastructure problems.

**Technologies:**
- Apply Well-architected framework on designs, good knowledge on services like VPC, EC2, ELB, ECS, Lambda, API-Gateway, RDS, DynamoDB and S3.
- Git
- SonarQube for code analysis
- Monitoring with CloudWatch, ELK Stack
- Collaborating on Scrum process with Asana tool, documentation with Confluence, Sharepoint

---

### Cryptocurrency Exchange System

**Team size: 20 members**  
**Duration: 10/2019 - 09/2023**  


**Description:**
A crypto exchange trading platform enables users to buy, sell, trade, and stake cryptocurrencies securely with features like order matching, market maker BOT, wallet integration, and staking rewards. It ensures KYC/AML compliance, multi-layer security, real-time analytics, and API support, providing a scalable and high-performance trading experience.

**Responsibilities:**
- Design and develop backend architecture
- Implement core functions such as order flows and Market Maker BOT
- Review team members’ code for quality and best practices
- Execute integration testing to ensure system stability
- Deploy and manage testing and production environments
- Monitor the system, including business functions and infrastructure
- Investigate, resolve, and report live issues
- Research and propose solutions for new features, including third-party integrations and cryptocurrency swap functions
- Plan, execute, and monitor project tasks using the Scrum model

**Technologies:**
- Java 1.8
- Spring Framework for Application and Dubbo Framework for Micro-service architecture
- Apache Zookeeper for Registry server
- mySQL, mongo, redis, rocketMQ
- AWS services for Deploy, Monitoring system and DBs
- FIX Protocol
- Integrate with Wallet, Exchange services like BitGo, oneZero
- Jenkins for CI/CD
- Docker

---

### University Management System Localization (Japan → Vietnam)

**Position: Developer**  
**Team size: 10 members**  
**Duration: 01/2016 - 09/2019**  


**Description:**
Adapted a Japan University Management System for Vietnamese universities, customizing enrollment, academics, faculty, and finance modules. Added multi-language support, localized grading, and compliance with Vietnam’s regulations, ensuring a smooth transition.

**Responsibilities:**
- Developed tools to extract, convert, and translate Japanese messages in the source code into Vietnamese.
- Developed tools to convert data from the old system to the new system.
- Developed new functions to support Vietnam university business processes.
- Created guideline documents to assist Vietnam university staff in using the system.
- Performed system testing and user testing based on requirements collected from Vietnam university staff.
- Managed Apache Tomcat server administration.
- Administered database servers and file servers.

**Technologies:**
- Java, JSP , Strut, JDBC
- Oracle
- Tomcat/ Apache
- Linux server

---

### Wedding Services Matching Platform

**Position: Developer -> Team Lead**  
**Team size: 50 members**  
**Duration: 03/2013 - 09/2016**  


**Description:**
A wedding services matching platform connecting users with service providers — wedding venues, bridal gown shops, catering, decoration, and more. Service providers register and upload their listings with images; users search and browse available options directly through the platform.

**Responsibilities:**

**As Developer:**
- Created detailed design documents based on functional requirements.
- Implemented new features and business logic in Java.
- Wrote and executed unit tests to ensure code quality.
- Supported integration testing across system modules.

**As Team Lead:**
- Communicated with Japanese clients to gather and clarify requirements.
- Mentored and supported team members in resolving technical issues.
- Coordinated task planning and progress tracking for the team.
- Managed deployment of application releases to Linux testing servers.

**Technologies:**
- Java, JSP, Strut, JDBC
- Oracle
- Tomcat/ Apache
- Linux server

---
