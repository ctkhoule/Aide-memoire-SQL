# Aide-memoire-SQL
SQL est l'acronyme de __Structured Query Language__. SQL est un langage de programmation standard spécialement conçu pour stocker, récupérer, gérer ou manipuler les données dans un __système de gestion de base de données relationnelle (SGBDR)__. 

SQL est le langage de base de données le plus largement implémenté et pris en charge par les systèmes de bases de données relationnelles populaires, tels que __MySQL__, __SQL Server__, __Oracle__, etc. Cependant, certaines fonctionnalités de la norme SQL sont implémentées différemment dans différents systèmes de base de données.

## Ce que vous pouvez faire avec SQL
Il y a beaucoup plus de choses que vous pouvez faire avec SQL :
- Vous pouvez créer une base de données.
- Vous pouvez créer des tables dans une base de données.
- Vous pouvez interroger ou demander des informations à partir d'une base de données.
- Vous pouvez insérer des enregistrements dans une base de données.
- Vous pouvez mettre à jour ou modifier des enregistrements dans une base de données.
- Vous pouvez supprimer des enregistrements de la base de données.
- Vous pouvez définir des autorisations ou un contrôle d'accès dans la base de données pour la sécurité des données.
- Vous pouvez créer des vues pour éviter de saisir des requêtes complexes fréquemment utilisées.
- etc.

## Une base de données relationnelle
Une base de données relationnelle est une base de données divisée en unités logiques appelées __tables__, où les tables sont liées les unes aux autres au sein de la base de données. La base de données relationnelle permet de diviser les données en unités logiques, plus petites et gérables pour une maintenance plus facile et de meilleures performances.

Les tables sont liées les unes aux autres via des __clés__ ou des __champs communs__ dans un système de base de données relationnelle, c'est pourquoi même si les données souhaitées peuvent exister dans plusieurs tables, vous pouvez facilement __joindre plusieurs tables__ pour obtenir un ensemble de données combiné à l'aide d'une seule requête.

## Quelques SGBDR
- [MySQL](https://www.mysql.com)
- [MariaDB](https://mariadb.org)
- [Oracle](https://www.oracle.com/database/technologies)
- [PostgreSQL](https://www.postgresql.org)
- [Microsoft SQL Server](https://www.microsoft.com/fr-fr/sql-server/sql-server-downloads)

## Utiliser Web SQL Database
SQL est utilisé pour communiquer avec la base de données, donc avant de commencer à expérimenter avec SQL, vous devez d'abord accéder à un système de base de données.

Vous pouvez tester ou exécuter la plupart des instructions SQL fournies à titre d'exemples tout au long des didacticiels, à l'aide de cet [éditeur SQL en ligne](https://www.tutorialrepublic.com/codelab.php?topic=sql&file=select-all). Cet éditeur SQL utilise __Web SQL Database__ pour stocker et accéder aux données côté client. Cependant, pour exécuter une instruction SQL, vous aurez besoin d'accéder à un système de gestion de base de données à part entière comme MySQL, SQL Server, etc.

__Web SQL Database__ vous permet de créer des bases de données SQL et d'effectuer des appels SQL côté client. Il est basé sur le moteur [SQLite](https://sqlite.org/index.html) populaire et __open source__. Web SQL est pris en charge par les navigateurs __Chrome, Opera et Safari__.


## Licence
Le projet est sous licence MIT - voir le fichier [LICENCE](https://github.com/ctkhoule/Aide-memoire-SQL/blob/main/LICENSE) pour plus de détails.
