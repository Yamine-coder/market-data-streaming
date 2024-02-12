# 📈 Market Data Streaming

Pipeline complet de traitement et de visualisation de données boursières en temps réel, construit avec **Apache Kafka**, **Apache Spark Streaming**, **MySQL**, **Grafana** et orchestré via **Docker**.

---

## 🧠 Objectif

Ce projet simule un système de surveillance des marchés financiers en temps réel, depuis l'ingestion de flux boursiers jusqu’à la visualisation dynamique. Il est conçu comme une architecture réutilisable dans des cas réels : finance, détection d’anomalies, monitoring applicatif.

---

## ⚙️ Architecture technique

API REST (ex: données boursières) → Kafka → Spark Streaming → MySQL → Grafana  
Toutes les briques sont déployées avec Docker.

---

## 🛠️ Stack utilisée

- **Kafka** – Ingestion des flux en temps réel  
- **Spark Streaming** – Traitement des données avec agrégation  
- **MySQL** – Stockage des données structurées  
- **Grafana** – Visualisation dynamique et monitoring  
- **Docker Compose** – Orchestration multi-conteneurs  
- **Python** – Producteur de messages Kafka (API simulée)

---

## 🚀 Lancement du projet

1. **Cloner le dépôt**

   `git clone https://github.com/Yamine-coder/market-data-streaming.git`

2. **Lancer l’environnement complet**

   `docker-compose up --build`

3. **Accéder aux services**

- Spark UI : `http://localhost:4040`  
- Grafana : `http://localhost:3000` (login : admin / admin)  
- MySQL : port `3306` (stockage des données boursières)

---

## 📊 Aperçu du Dashboard Grafana

![Dashboard Grafana](./images/grafana-preview.png)

> Visualisation en temps réel des indicateurs de marché (prix, variation, volume...).

---

## 📂 Contenu du dépôt

- `producer/` → Producteur Kafka en Python
- `spark/` → Script Spark Streaming pour traitement des flux
- `grafana/` → Fichiers de configuration Grafana
- `mysql/` → Init de la base de données
- `docker-compose.yml` → Orchestration des services
- `README.md`

---

## 💼 Cas d’usage métier

- 🔍 Surveillance temps réel des données de marché
- 📈 Détection d’anomalies sur les cours boursiers
- ⚙️ Modèle d’architecture pour projets Data/IA/DevOps temps réel

---

## 👤 Auteur

**Yamine Moussaoui**  
Consultant en Solutions Data & IA  
🔗 [GitHub](https://github.com/Yamine-coder) · [LinkedIn](https://www.linkedin.com/in/yamine-moussaoui-672a25205/)

---

## 🪪 Licence

Projet open source sous licence MIT — libre d’utilisation et de modification.
