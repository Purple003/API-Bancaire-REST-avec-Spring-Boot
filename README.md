# 🏦 API Bancaire REST - Spring Boot

[![Spring Boot](https://img.shields.io/badge/Spring%20Boot-3.2-green.svg)](https://spring.io/projects/spring-boot)
[![Java](https://img.shields.io/badge/Java-17-orange.svg)](https://openjdk.org/)
[![H2 Database](https://img.shields.io/badge/H2-Database-blue.svg)](http://www.h2database.com)

##  Contexte du Projet
Ce projet a été développé dans le cadre d'un TP Spring Boot visant à créer une API REST complète pour la gestion de comptes bancaires.

##  Fonctionnalités Implémentées

###  API REST Complète
- **GET /banque/comptes** - Liste tous les comptes (JSON/XML)
- **GET /banque/comptes/{id}** - Récupère un compte par ID
- **POST /banque/comptes** - Crée un nouveau compte
- **PUT /banque/comptes/{id}** - Met à jour un compte
- **DELETE /banque/comptes/{id}** - Supprime un compte

###  Support Multi-Format
- Content Negotiation avec headers `Accept` et `Content-Type`
- Support simultané JSON et XML

###  Base de Données
- Base H2 en mémoire avec console d'administration
- Initialisation automatique des données via CommandLineRunner

##  Captures d'Écran de Validation

### Tests API avec Postman
<img width="1322" height="718" alt="Screenshot 2025-11-02 210440" src="https://github.com/user-attachments/assets/f8500b3f-284d-46d2-8b98-405e126066f0" />
<img width="1316" height="688" alt="Screenshot 2025-11-02 210704" src="https://github.com/user-attachments/assets/c749c9d9-2263-4abe-a949-141ccb35d278" />
<img width="1303" height="751" alt="Screenshot 2025-11-02 211310" src="https://github.com/user-attachments/assets/63e84a1a-1c75-4e5d-9d67-80dcf3ccd636" />
<img width="1358" height="720" alt="Screenshot 2025-11-02 211603" src="https://github.com/user-attachments/assets/5daaa45d-2b01-4393-90e9-5c35a62aa26a" />
<img width="1317" height="629" alt="Screenshot 2025-11-02 212359" src="https://github.com/user-attachments/assets/2f3bfcc3-a953-4e34-9895-3a4697b19f6b" />
<img width="1338" height="670" alt="Screenshot 2025-11-02 212519" src="https://github.com/user-attachments/assets/47906e26-86a4-4fe6-8ddd-b2dd85345827" />
<img width="819" height="782" alt="Screenshot 2025-11-02 212926" src="https://github.com/user-attachments/assets/58a0a1a0-4f18-4944-b44f-a5b4d3ae8f0b" />
<img width="1327" height="668" alt="Screenshot 2025-11-02 213301" src="https://github.com/user-attachments/assets/3c9bc6dc-709c-4537-9a87-f21f2212529f" />

*Validation complète des opérations CRUD*

### Console H2 Database
<img width="691" height="724" alt="Screenshot 2025-11-02 214743" src="https://github.com/user-attachments/assets/fae68f0e-c3c0-495c-abfd-80a13f4dde79" />

*Accès à la base de données H2*

### Données Persistantes
<img width="1900" height="822" alt="Screenshot 2025-11-02 214942" src="https://github.com/user-attachments/assets/b886bff6-e805-4bb0-bb93-81579d98ba5d" />
*Visualisation des données en base*

### Réponse API JSON
<img width="1336" height="629" alt="Screenshot 2025-11-02 205820" src="https://github.com/user-attachments/assets/88c6cbb0-80ee-42c7-b2ae-b335574891d6" />
*Format JSON validé*

### Réponse API XML
<img width="1316" height="707" alt="Screenshot 2025-11-02 210222" src="https://github.com/user-attachments/assets/d1f280a4-51f1-4e75-b77d-0d81c6c63d66" />
*Format XML validé*


## 🛠 Technologies Utilisées
- **Spring Boot 3.2+** - Framework principal
- **Spring Data JPA** - Persistance des données
- **H2 Database** - Base de données embarquée
- **Maven** - Gestion des dépendances

##  Résultats des Tests

### Tests Fonctionnels Réussis
- **CRUD Complet** - Toutes les opérations validées
- **Formats JSON/XML** - Négociation de contenu fonctionnelle
- **Gestion d'Erreurs** - Codes HTTP appropriés (200, 201, 404)
- **Persistance** - Données cohérentes entre API et base H2

###  Validation Technique
- Console H2 accessible sur `http://localhost:8082/h2-console`
- API opérationnelle sur `http://localhost:8082/banque/comptes`
- Temps de réponse optimaux (< 200ms)
- Structure MVC respectée


##  Structure du Projet

```
src/main/java/ma/rest/spring/
├──  Application.java
├──  entities/
│   ├── Compte.java
│   └── TypeCompte.java
├──  repositories/
│   └──  CompteRepository.java
└──  controllers/
    └──  CompteController.java
```

**Description des composants :**
- **`Application.java`** - Classe principale Spring Boot
- **`Compte.java`** - Entité JPA représentant un compte bancaire
- **`TypeCompte.java`** - Enumération des types de compte (EPARGNE/COURANT)
- **`CompteRepository.java`** - Interface Spring Data JPA pour la persistance
- **`CompteController.java`** - Contrôleur REST exposant les endpoints API

##  Points Forts du Projet

1. **Architecture RESTful** respectée
2. **Code propre et structuré** suivant les bonnes pratiques Spring
3. **Gestion d'erreurs** implémentée
4. **Tests complets** avec Postman
5. **Documentation** complète des endpoints

##  Conclusion
Ce TP démontre une maîtrise complète du développement d'API REST avec Spring Boot, incluant la persistance JPA, la gestion des formats multiples, et les tests d'intégration.

##  Auteur

**Arroche Aya**
