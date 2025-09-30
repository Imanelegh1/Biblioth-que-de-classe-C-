# Biblioth-que-de-classe-C-
Bibliothèque de classe C#
MonitoringPlus est une bibliothèque et une application console développées dans le cadre d’un projet de stage.
Elle permet de :

Effectuer des tests de services WCF REST (appels interactifs ou en batch).

Simuler plusieurs utilisateurs virtuels pour tester la charge.

Collecter et enregistrer automatiquement les résultats (succès, erreurs, temps d’exécution, etc.) dans une base de données SQL Server.

Fournir un suivi des performances et faciliter l’analyse des comportements en temps réel.

 Technologies utilisées

Langage : C# (.NET Framework 4.8)

Environnement de développement : Visual Studio

Base de données : SQL Server

Outils de test : Postman (pour la validation initiale des API REST)

 Structure du projet

MonitoringPlus/ → Bibliothèque principale contenant la logique de monitoring et de test.

MonitoringPlus.Console/ → Application console permettant d’exécuter des campagnes de tests.

SQL/ → Scripts SQL pour la création de la table Logs et la configuration de la base.

 Fonctionnalités principales

Exécution de méthodes WCF avec suivi des performances.

Journalisation automatique dans une table SQL (Logs).

Génération de métriques : temps de réponse, code retour, message, exception éventuelle.

Support de tests multi-utilisateurs (utilisateurs virtuels).

Mode interactif et batch.

 Exemple de table Logs
Methode	Code	Message	Exception	Timestamp	VirtualUsers	MachineName
UpdateUser	200	OK	NULL	2025-09-01 12:30	3	PC-TEST
 Utilisation



Ouvrir le projet dans Visual Studio.

Configurer la chaîne de connexion SQL Server dans App.config.

Lancer l’application console et suivre les instructions (nombre d’appels, utilisateurs virtuels, etc.).
