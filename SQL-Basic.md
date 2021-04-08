# Les bases de SQL
Dans ce didacticiel vous apprendrez les bases de SQL.

Une instruction SQL est composée d'une séquence de __mots-clés, d'identificateurs__, etc. terminée par un point-virgule __(;)__.

Les mots clés SQL sont insensibles à la casse. Cependant, les noms de base de données et de table peuvent être sensibles à la casse en fonction du système d'exploitation. En général, les plates-formes __Unix__ ou __Linux__ sont sensibles à la casse, contrairement aux plates-formes __Windows__.

__Conseil : Il est recommandé d'écrire les mots-clés SQL en majuscules, pour les différencier des autres textes dans une instruction SQL pour une meilleure compréhension.__

## Créer et sélectionner une base de données 
Avant de faire quoi que ce soit avec les données, nous devons d'abord créer une base de données. Nous supposons que vous avez déjà un [SGBDR](https://github.com/ctkhoule/Aide-memoire-SQL#quelques-sgbdr).

L'instruction SQL `CREATE DATABASE` est utilisée pour créer une base de données.

    CREATE DATABASE nom_base;
    
Par exemple créons une base de données dans __MySQL__ à l'aide de l'outil de ligne de commande.

- __Etape 01 : Appeler l'outil de ligne de commande MySQL__

Pour appeler la ligne de commande MySQL, nous devons d'abord nous connecter au serveur MySQL. Pour vous connecter en tant qu'utilisateur `root`, tapez la commande suivante dans le terminal et appuyez sur Entrée. Il vous sera demandé votre __mot de passe__. Entrez votre mot de passe et appuyez sur Entrée, s'il est correct, l'invite `mysql>` apparaîtra, via laquelle vous pourrez émettre des instructions SQL et afficher les résultats.

    mysql -u root -p 

- __Etape 02 : Création d'une base de données MySQL__

Maintenant, exécutez la commande suivante pour créer la base de données nommée __mybase__.
    
    CREATE DATABASE mybase;
 
Si vous essayez de créer une base de données qui existe déjà, vous obtiendrez un __message d'erreur__. Pour éviter cela dans MySQL, vous pouvez utiliser une clause facultative `IF NOT EXISTS` comme suit :

    CREATE DATABASE IF NOT EXISTS mybase;
    
- __Etape 03 : Sélectionner la base de données__

Tapez la commande suivante (`USE nom_base`) et appuyez sur Entrée. Vous verrez la sortie "__Database changed__". Maintenant la base de données est sélectionnée comme base de données par défaut pour toutes les opérations futures.

    USE mybase;

__Conseil : Pour afficher l'ensemble des bases de données existantes sur le serveurm vous pouvew exécuter l'instruction `SHOW DATABASES` sur la ligne de commande.__
