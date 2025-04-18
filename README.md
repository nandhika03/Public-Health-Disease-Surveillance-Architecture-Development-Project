# 🏥 Public Health Disease Surveillance Architecture

This project demonstrates the end-to-end development of a disease surveillance system using synthetic health data, OpenEMR, FHIR standards, and HAPI-FHIR integration. It aims to simulate a healthcare IT infrastructure that supports real-time outbreak monitoring and secure health data exchange across hospitals.

## 📌 Objectives

- Understand and implement core components of Healthcare Information Technology (HIT)
- Simulate patient records and disease outbreaks (e.g., COVID-19)
- Implement the FHIR standard using the HAPI-FHIR server
- Enable secure data exchange using POSTMAN and Swagger UI

## 🛠️ Architecture Steps

### 1. Virtual Machine Configuration
- Created 5 VMs: 4 hospitals + 1 Health Information Exchange (HIE)
- Configured static IPs on VMware vSphere

### 2. OpenEMR Installation
- Installed OpenEMR 6.0.1 on Ubuntu servers
- Secured systems via firewall (`ufw`), Apache, and PHP hardening

### 3. Synthetic Data Generation
- Used [Synthea](https://github.com/synthetichealth/synthea) to simulate patient and syndromic data for each hospital
- Included COVID-19 simulation in generated FHIR data

### 4. HAPI-FHIR Server Setup
- Deployed HAPI-FHIR server on HIE VM using Docker
- Configured via custom `application.yaml` file

### 5. FHIR Data Exchange via POSTMAN
- Used POSTMAN for testing FHIR API endpoints (e.g., `Practitioner`)
- Explored RESTful API endpoints via Swagger UI

## 🧪 Technologies Used

- VMware vSphere
- Ubuntu Server
- OpenEMR 6.0.1
- Synthea
- HAPI-FHIR (Dockerized)
- POSTMAN
- BIG-IP Edge VPN

## 🚧 Challenges Faced

- Initial difficulty setting up VMs and network configurations
- Understanding new tools like Docker and Synthea CLI

## ✅ Outcomes

- Developed a functional HIT simulation with hospital-level EHRs
- Enabled real-time surveillance using synthetic outbreak data
- Demonstrated secure data interoperability using FHIR APIs

## 📎 Resources

- [Synthea Releases](https://github.com/synthetichealth/synthea/releases)
- [HAPI-FHIR Docs](https://hapifhir.io)
- [Cerner FHIR Reference](https://fhir.cerner.com)

---

> 📍 *This project was developed as a learning module to better understand the infrastructure and protocols involved in public health surveillance systems.*
