# Rapport TPJavaPipeLine-ZayemHafsa


### Introduction
Ce TP consiste à mettre en place un pipeline CI/CD complet
avec Jenkins, GitHub Webhook et Docker.

### Architecture
GitHub (push) → Webhook → ngrok → Jenkins → Pipeline CI/CD

## Technologies
- Java 21 / Maven
- Jenkins 2.528.2 (Docker)
- GitHub Webhook
- ngrok
- Docker


## 1️ Projet Maven
<img width="1918" height="1033" alt="mvn-compile" src="https://github.com/user-attachments/assets/c1744027-37cf-44f4-88d8-e36ee0d65358" />
-
<img width="1917" height="1036" alt="mvn install1" src="https://github.com/user-attachments/assets/b1b3f60a-21c9-429e-a6df-1f1a3d76b07f" />
-
<img width="1913" height="1005" alt="mvn clean intall" src="https://github.com/user-attachments/assets/afe23ba1-4ab4-451b-b000-b3d854303885" />

## 2️ Jenkins Dashboard
<img width="1335" height="100" alt="d j" src="https://github.com/user-attachments/assets/d4d7ac38-8fbd-4200-a42a-cb56eee84cea" />
-
<img width="1918" height="1060" alt="d jnks" src="https://github.com/user-attachments/assets/8138d96e-9546-4a66-9447-232cf0b36335" />
-
<img width="1930" height="931" alt="jenkins-dashboard" src="https://github.com/user-attachments/assets/bc8642a0-2fb1-4b93-b0c2-5850e8336d39" />

## 3️ Plugin GitHub Integration
<img width="1417" height="517" alt="jenkins-plugin" src="https://github.com/user-attachments/assets/09498212-1ff8-4e7b-a10f-cebb1e7c8760" />

## 4️ ngrok tunnel
<img width="1057" height="327" alt="ngrok-tunnel" src="https://github.com/user-attachments/assets/cad08e07-1fb5-4431-9e00-28f85cfec04a" />

## 5️ Webhook GitHub
<img width="1375" height="927" alt="webhook-config" src="https://github.com/user-attachments/assets/81922554-962f-4d06-80a8-037615d99df7" />
-
<img width="1007" height="922" alt="mapping" src="https://github.com/user-attachments/assets/96546fd4-c09d-463b-b7f3-59a06eb42b13" />


## 6️ Pipeline Jenkins

<img width="1436" height="162" alt="mlt" src="https://github.com/user-attachments/assets/b4aac574-350c-49f0-9414-addb4be79514" />
-
<img width="1765" height="917" alt="conf" src="https://github.com/user-attachments/assets/3cd5e40d-ebd8-41c0-8bc2-28e01dc03ad6" />
-
<img width="1918" height="908" alt="Scan Repo" src="https://github.com/user-attachments/assets/8e5d556c-1f5a-4e20-aa6e-6b20c2c2fed1" />
-
<img width="1918" height="927" alt="jk log" src="https://github.com/user-attachments/assets/30763698-e224-478f-8a42-ea6793a5e21f" />
-
<img width="1645" height="828" alt="wh" src="https://github.com/user-attachments/assets/3006a18b-3896-48cd-bf69-83db03d289e5" />
-
<img width="1157" height="898" alt="v m" src="https://github.com/user-attachments/assets/e12c43f6-823a-4dd7-823d-b5f6ed3d53ed" />
-
<img width="1918" height="896" alt="v 6" src="https://github.com/user-attachments/assets/2a272aa7-3913-4dea-b689-befbc982d4b4" />

---


### Étapes réalisées
1. Création d'un projet Java Maven compilant sans erreur
2. Création du Jenkinsfile avec 4 stages : Checkout, Build, Test, Package
3. Configuration de ngrok pour exposer Jenkins local à GitHub
4. Création du Webhook GitHub pour déclencher Jenkins automatiquement
5. Création du Multibranch Pipeline Jenkins
6. Vérification du déclenchement automatique après git push

### Résultats
Pipeline exécuté avec succès (Build #5 et #6). Tous les stages sont verts ✅.
Chaque push sur GitHub déclenche automatiquement le build Jenkins.

### Conclusion
Le pipeline CI/CD fonctionne correctement. L'intégration
GitHub + Jenkins + Docker permet une livraison continue automatisée.

