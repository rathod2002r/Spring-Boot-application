# Spring-Boot-application
# 💼 Financial Advisor Management System

This project is a Spring Boot backend system designed to help financial advisors manage their clients and their investment portfolios. It supports full CRUD operations on advisors, clients, portfolios, and securities.

---

## 🚀 Features

- Manage multiple financial advisors
- Create, update, delete clients under each advisor
- Each client has a portfolio
- Each portfolio contains multiple securities
- Built with Java Spring Boot and JPA (Hibernate)
- Uses relational database (MySQL/PostgreSQL supported)
- Exposes a RESTful API for React dashboard integration

---

## 🏗️ Data Model Overview

### Entities
- **FinancialAdvisor** – has many Clients
- **Client** – belongs to one FinancialAdvisor, has one Portfolio
- **Portfolio** – belongs to one Client, has many Securities
- **Security** – belongs to one Portfolio

### Relationships
- One-to-many: FinancialAdvisor → Clients
- One-to-one: Client → Portfolio
- One-to-many: Portfolio → Securities

---

## 🛠️ Technologies Used

- Java 17
- Spring Boot 3.x
- Spring Data JPA (Hibernate)
- Maven
- MySQL / PostgreSQL
- IntelliJ IDEA

---

## 📦 Getting Started

### Prerequisites

- Java 17+
- Maven 3.8+
- IntelliJ IDEA
- MySQL or PostgreSQL running locally

### Clone the Repository

```bash
git clone https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git
cd YOUR_REPO_NAME
