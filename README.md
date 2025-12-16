# TP BPM/BPEL - Business Process Management Project

A BPMN (Business Process Model and Notation) project built with **Bonita BPM** platform for modeling and automating business processes.

## 📋 Project Overview

This project implements a **Purchase Order Process** (Processus Achat) using BPMN 2.0 standards. It models a complete order management workflow involving multiple services:

- **Service Client** - Customer service for identity verification
- **Service Ventes** - Sales service for stock availability control
- **Service Livraison/Paiement** - Delivery and payment service
- **Service Comptabilité** - Accounting service for order creation
- **Banque/Livraison** - Bank and delivery handling
- **Service Mail** - Email notification service

## 🏗️ Project Structure

```
BPEL_BPMN/
├── diagram_1.bpmn          # Main BPMN diagram for order process
├── pom.xml                 # Parent Maven configuration
├── app/
│   ├── pom.xml             # Application Maven configuration
│   ├── diagrams/           # Bonita process diagrams
│   │   └── Processus_Achat-1.0.proc
│   ├── environements/      # Environment configurations
│   │   ├── Production.xml
│   │   └── Qualification.xml
│   ├── organizations/      # Organization definitions
│   │   └── ACME.xml
│   └── web_page/           # Web forms and UI
│       └── newForm2/
│           ├── newForm2.json
│           └── assets/
```

## 🛠️ Technologies Used

- **Bonita BPM** 10.2.0 - Business Process Management Platform
- **BPMN 2.0** - Business Process Model and Notation Standard
- **Maven** - Build and dependency management
- **Groovy** - Scripting language for process automation
- **Java** - Backend runtime environment

## 📦 Dependencies

- Bonita Common Engine
- Groovy (JSON, XML, NIO, DateTime, SQL support)

## 🚀 Getting Started

### Prerequisites

- Java JDK 11 or higher
- Maven 3.6+
- Bonita Studio 10.2.0

### Installation

1. Clone the repository
2. Import the project into Bonita Studio
3. Build with Maven:
   ```bash
   mvn clean install
   ```

### Running the Process

1. Open Bonita Studio
2. Import the project
3. Open `Processus_Achat-1.0.proc` from the diagrams folder
4. Run the process in the appropriate environment (Qualification/Production)

## 📊 Process Flow

1. **Order Request Reception** - Customer submits an order
2. **Identity Verification** - Customer authentication check
3. **Stock Availability Control** - Check if items are in stock
4. **Payment Processing** - Handle payment transaction
5. **Order Creation** - Create the order in the system
6. **Shipping Scheduling** - Program the delivery
7. **Email Notification** - Send confirmation email to customer

## 👥 Authors

| Name                  | Role      |
| --------------------- | --------- |
| **Aymen Lamkhanet**   | Developer |
| **Hibat-Allah Jamil** | Developer |

## 📄 License

This project is developed as part of a BPM/BPEL practical work (TP).

---

_Made with ❤️ by Aymen Lamkhanet & Hibat-Allah Jamil_
