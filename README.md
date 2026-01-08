# Zabbix Monitoring on AWS with Docker

## Description
Ce projet présente la mise en œuvre d’une solution de supervision avec **Zabbix**, déployée sur **AWS** à l’aide de **Docker**.  
L’objectif est de surveiller des machines **Linux et Windows** en temps réel, de centraliser les métriques système et de gérer automatiquement les alertes.

---

## Architecture

### Diagramme général
AWS EC2
├─ Zabbix Server (Docker)
|
│ ├─ PostgreSQL (Docker)
|
│ └─ Zabbix Web Frontend (Docker)
|
├─ Client Linux (Zabbix Agent)
|
└─ Client Windows (Zabbix Agent)


### Composants principaux
- **Zabbix Server** : Collecte et centralise toutes les données des agents.
- **Zabbix Web Frontend** : Interface web pour la visualisation et la configuration.
- **PostgreSQL** : Base de données pour stocker les métriques et la configuration.
- **Zabbix Agents** : Logiciels installés sur Linux et Windows pour envoyer les métriques.
- **AWS EC2** : Hébergement des instances serveur et clients.

---

## Technologies utilisées
- **Cloud** : AWS EC2  
- **Supervision** : Zabbix 7.4  
- **Conteneurisation** : Docker & Docker Compose  
- **Base de données** : PostgreSQL 15  
- **Clients surveillés** : Linux (Ubuntu 22.04), Windows 10/11  
- **Scripts** : Bash pour Linux, PowerShell pour Windows  

---

## Déploiement du projet

### 1. Cloner le dépôt

https://github.com/AyoubFanaoui/zabbix-aws-docker-monitoring.git
cd zabbix-aws-docker-monitoring

3. Lancer les services Docker
docker compose up -d

