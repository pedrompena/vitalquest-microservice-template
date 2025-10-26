# 📘 VitalQuest Microservice Template

<!--toc:start-->
- [📘 VitalQuest Microservice Template](#📘-vitalquest-microservice-template)
  - [✨ Key Features](#key-features)
  - [🚀 Quick Start](#🚀-quick-start)
    - [Clone the repo](#clone-the-repo)
    - [Run locally (dev profile)](#run-locally-dev-profile)
    - [Build & run with Docker](#build-run-with-docker)
  - [🧩 Suggested Usage](#🧩-suggested-usage)
  - [📦 Dependencies (from Gradle)](#📦-dependencies-from-gradle)
<!--toc:end-->

A colorful, production-ready Spring Boot microservice template following a hexagonal architecture (ports & adapters) 🎯.
Designed to kickstart new microservices with Gradle, Docker, dev profiles, PostgreSQL, and Prometheus metrics.

## ✨ Key Features

- 🏗 Hexagonal architecture (clear separation between domain, application, and infrastructure)

- ☕ Java 25 + Spring Boot 3.5.7

- 🐘 PostgreSQL as the primary database

- 📊 Prometheus metrics via Micrometer

- 🐳 Dockerfile and .dockerignore ready for containerization

- 📁 Layered project structure for fast bootstrapping

- ⚡ Dev tools and sensible defaults for logging, validation, and health checks

- 🧪 Testing setup with Testcontainers (PostgreSQL & Kafka) and JUnit 5

- 🛠 CI/CD-ready structure (placeholders for GitHub Actions or other pipelines)

## 🚀 Quick Start

### Clone the repo

```
git clone git@github.com:pedrompena/vitalquest-microservice-template.git
cd vitalquest-microservice-template
```

### Run locally (dev profile)

```
./gradlew bootRun --args='--spring.profiles.active=dev'
```

### Build & run with Docker

```docker build -t vitalquest/ms-template:latest .
docker run -p 8080:8080 vitalquest/ms-template:latest
```

## 🧩 Suggested Usage

Use this repository as a starting point for all VitalQuest microservices. Replace example domain models and adapters with your real implementations, configure your PostgreSQL connection, and plug in observability tools like Prometheus.

## 📦 Dependencies (from Gradle)

spring-boot-starter-web 🌐

spring-boot-starter-data-jpa 🗄

spring-boot-starter-validation ✅

spring-boot-starter-actuator ⚙️

spring-cloud-starter-config 🔧

spring-kafka 🎵

micrometer-registry-prometheus 📊

postgresql 🐘

spring-boot-devtools (development only) 🛠

Testing: spring-boot-starter-test, testcontainers (PostgreSQL, Kafka), JUnit 5 🧪
