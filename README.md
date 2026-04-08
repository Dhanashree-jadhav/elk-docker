# ELK Stack (Elasticsearch + Kibana) using Docker Compose

## 📌 Overview

This project sets up a basic **ELK stack** using Docker Compose, including:

* **Elasticsearch** – for storing and searching data
* **Kibana** – for visualizing data

---

## 🚀 Services

### 1. Elasticsearch

* Runs version `8.12.0`
* Configured in **single-node mode**
* Security disabled for easy local setup
* Accessible at: `http://localhost:9200`

### 2. Kibana

* Runs version `8.12.0`
* Connects to Elasticsearch using service name
* Accessible at: `http://localhost:5601`

---

## ⚙️ Configuration Highlights

* Uses Docker Compose version `3.8`
* Both services are connected via a custom network `elk`
* Kibana depends on Elasticsearch to start first

---

## ▶️ How to Run

```bash
docker-compose up -d
```

---

## 🌐 Access

* Elasticsearch: http://localhost:9200
* Kibana: http://localhost:5601

---

## 🧠 Notes

* This setup is for **local development/testing only**
* Security is disabled for simplicity
* Can be extended with Logstash or Filebeat for log processing

---
