
# I. Introduction
La connexion entre Kafka et MySQL via Kafka Connect permet de transférer des données en temps réel de MySQL à Kafka. Kafka Connect fournit un framework qui simplifie l'écriture et la configuration des connecteurs pour les sources et les destinations de données, et permet d'extraire, de transformer et de charger les données de manière efficace.

En utilisant le connecteur JDBC fourni par Kafka Connect, il est possible de configurer une source de données MySQL et de transférer les données de la base de données vers un ou plusieurs topics Kafka. Ainsi, les données provenant de MySQL sont immédiatement disponibles pour les applications Kafka qui peuvent les traiter, les agréger ou les stocker pour une utilisation ultérieure.

La connexion entre Kafka et MySQL via Kafka Connect est donc particulièrement utile pour les applications nécessitant une intégration en temps réel des données provenant d'une base de données relationnelle, ou pour les cas d'utilisation nécessitant un traitement distribué et parallèle des données, tels que la surveillance en temps réel, le traitement de flux, ou encore l'analyse de données.

### A. Présentation de Kafka Connect :  <br />
Kafka Connect est un outil open source de streaming de données qui permet de connecter facilement des sources de données externes à un cluster Apache Kafka. Il permet de transférer des données de manière fiable, scalable et efficace entre des systèmes hétérogènes, tels que des bases de données, des systèmes de fichiers, des applications ou des services web.
![image](https://github.com/Barhoumi-mohamedali/kafka-mysql/assets/1130140/7515d303-1e7e-4ee0-b83c-a97240053785)
 <br />
### B. Explication de la connexion entre Kafka et MySQL via Kafka Connect <br />
Kafka Connect permet de connecter facilement des sources de données externes, telles que des bases de données, à un cluster Apache Kafka. Pour connecter MySQL à Kafka via Kafka Connect, on peut utiliser le connecteur JDBC (Java Database Connectivity).

Le connecteur JDBC permet de lire des données de MySQL en temps réel et de les écrire dans un topic Kafka spécifié. Le connecteur surveille les modifications apportées à la base de données MySQL en utilisant des journaux de transactions et écrit les modifications dans Kafka. Les données écrites dans Kafka sont structurées sous forme de messages JSON ou Avro, qui peuvent être traités par des applications Kafka pour effectuer des analyses en temps réel.

La configuration du connecteur JDBC nécessite de spécifier les paramètres de connexion à la base de données MySQL, tels que l'URL de connexion, le nom d'utilisateur et le mot de passe. Il faut également spécifier le topic Kafka dans lequel écrire les données.

Une fois le connecteur configuré et lancé, il permet de transférer des données de MySQL à Kafka en temps réel, de manière fiable et évolutive. Cette connexion entre Kafka et MySQL via Kafka Connect peut être utilisée pour une variété de cas d'utilisation, tels que l'ingestion de données en temps réel, la synchronisation de données entre différents systèmes et la diffusion de données à des applications en aval pour une analyse en temps réel.




# II. Prérequis
A. Installation de Kafka
B. Installation de MySQL
C. Installation de Kafka Connect

# III. Configuration de MySQL
A. Création d'une base de données
B. Création d'une table
C. Ajout de données dans la table

# IV. Configuration de Kafka Connect
A. Configuration de la source MySQL
B. Configuration du connecteur JDBC
C. Configuration de la destination Kafka
D. Configuration du connecteur Kafka

# V. Lancement du connecteur Kafka
A. Vérification de la connexion
B. Visualisation des données dans Kafka

# VI. Conclusion
A. Récapitulation des étapes
B. Explication de l'intérêt de la connexion entre Kafka et MySQL via Kafka Connect
C. Pistes d'amélioration du tutoriel
