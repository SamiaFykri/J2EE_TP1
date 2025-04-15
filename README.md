# J2EE_TP1
# DAO avec Injection de Dépendances et Couplage Faible en Java

## Introduction

Ce projet a pour but de démontrer l'application des principes d'injection de dépendances (DI) et de couplage faible en Java, à l'aide de DAO (Data Access Object) pour gérer l'accès aux données. Le projet permet de basculer entre deux méthodes d'accès aux données : une implémentation DAO traditionnelle (avec une base de données locale) et une implémentation DAO basée sur un Web Service.

L'objectif principal est de montrer comment injecter les dépendances de manière flexible, tout en maintenant un faible couplage entre les différentes couches de l'application.

## Objectifs du TP

- Appliquer les principes de l'injection de dépendances et du couplage faible.
- Mettre en place une solution qui permet de basculer  entre un DAO BD et un DAO Web Service.
- Utiliser des interfaces pour assurer une abstraction entre les différentes couches de l'application.


### Injection de Dépendances et Couplage Faible

L'injection de dépendances est réalisée manuellement en Java. Le projet repose sur des interfaces pour définir les contrats d'accès aux données. L'implémentation de l'interface `IDao` peut être soit un DAO classique (`DaoImpl`), soit un DAO Web Service (`DaoImplV2`), et l'implémentation choisie est injectée dans la couche métier.

### Basculement entre DAO classique et DAO Web Service

Le basculement entre les deux implémentations de DAO est effectué via une configuration dans la classe `AppConfig.java`. En fonction de la configuration, l'application utilisera l'une ou l'autre des implémentations.


### Fichiers clés du projet

IDAO.java
DAOimlp.java
DAOimplV2.java
IMETIER.java
IMetierImpl.java
Presentation1.java
Presentation2.java
config.txt

### Execution

<img width="557" alt="tp1" src="https://github.com/user-attachments/assets/a74ab59f-811b-4fa2-8da8-21c96b79012e" />

