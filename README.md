# Projet_Kafka_Weather

Ce projet permet de récupérer des données météorologiques en temps réel à partir de l'API OpenWeather et de les envoyer à un serveur Kafka. Les données sont ensuite traitées par un consommateur utilisant Apache Spark Streaming, et les résultats sont envoyés vers un autre topic Kafka.

Le projet comprend deux parties principales :

Un producteur Kafka qui récupère des données météorologiques pour plusieurs villes et les envoie à Kafka.

Un consommateur Kafka utilisant Apache Spark pour traiter les données en temps réel et effectuer des calculs additionnels.

Le code implémente un pipeline de données en temps réel utilisant Kafka et Apache Spark pour collecter, traiter et analyser des informations météorologiques. Un producteur Kafka récupère les données météorologiques pour plusieurs villes via l'API OpenWeather, les sérialise en JSON et les envoie dans un topic Kafka (tp-meteo). Un consommateur Kafka, basé sur Apache Spark Streaming, lit ces données en temps réel depuis le topic Kafka, les parse, applique des transformations et calculs comme l'index de chaleur et l'index de sévérité, puis les envoie dans un autre topic Kafka (tp-meteo-final). Ce système permet d’analyser les conditions météorologiques à travers différentes villes en continu et en temps réel, facilitant ainsi des analyses plus complexes ou des alertes.







