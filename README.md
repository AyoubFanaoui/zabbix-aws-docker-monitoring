# Zabbix Monitoring on AWS with Docker

## Description
Ce projet présente la mise en œuvre d’une solution de supervision avec **Zabbix**, déployée sur **AWS** à l’aide de **Docker**.  
L’objectif est de surveiller des machines **Linux et Windows** en temps réel, de centraliser les métriques système et de gérer automatiquement les alertes.

---

## Architecture

### Diagramme général
<img width="342" height="205" alt="image" src="https://github.com/user-attachments/assets/46d7995a-7a37-4cb5-89f4-4c271f26402d" />


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
<img width="745" height="372" alt="image" src="https://github.com/user-attachments/assets/515b3f39-68a2-4dfc-9906-89b8cbdb75bd" />


