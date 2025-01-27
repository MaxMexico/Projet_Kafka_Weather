# Projet_Kafka_Weather

Ce projet permet de récupérer des données météorologiques en temps réel à partir de l'API OpenWeather et de les envoyer à un serveur Kafka. Les données sont ensuite traitées par un consommateur utilisant Apache Spark Streaming, et les résultats sont envoyés vers un autre topic Kafka.

Le projet comprend deux parties principales :

Un producteur Kafka qui récupère des données météorologiques pour plusieurs villes et les envoie à Kafka.
Un consommateur Kafka utilisant Apache Spark pour traiter les données en temps réel et effectuer des calculs additionnels.