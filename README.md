GRR
===================

**Requiert :**

PHP : > 7.0 && <= 7.3; nécessite au moins les modules php-gd, php-mbstring, php-mysqli, php-mysqlnd, php-xml (*)
MySQL: > 5.4 && < 5.6, compatibilité vraisemblable avec MySQL 5.7

http://grr.devome.com/

GRR est un outil de gestion et de réservation de ressources. **GRR** est une adaptation d'une application **MRBS**.

----------

Installation
-------------

Pour obtenir une description complète de la procédure d'installation, veuillez vous reporter au fichier "**INSTALL.txt**".

Pour une installation simplifiée, décompressez simplement cette archive sur un serveur, et indiquez l'adresse où se trouvent les fichiers extraits dans un navigateur (ex: http://www.monsite.fr/grr).

>Préalables pour l'installation automatisée :
>disposer d'un espace FTP sur un serveur, pour y transférer les fichiers
>disposer d'une base de données MySQL (adresse du serveur MySQL, login, mot de passe)


Mise à jour
-------------

La version 4 est en cours de développement il est déconseillé de mettre à jour vos sites en production.

Vous devez faire une mise à jour classique en suivant la procédure habituelle ( https://site.devome.com/fr/grr/telechargement/category/2-informations-documentations?download=2:mise-a-jour-de-votre-grr) . Attention PHP 7 minimum !

En plus de la mise à jour classique, veuillez rendre accessible le dossier "personnalisation" en écriture. C'est désormais dans ce dossier que vos personnalisations seront sauvegardées.

- Editer votre fichier connect.inc.php et ajouter la ligne suivante en y mettant 12 caractères alphanumériques
	$hashpwd1="ici vos 12 caractères";
- Déplacer votre fichier connect.inc.php dans personnalisation
- Si vous possédez des modules vous devez les déplacer dans le dossier "personnalisation/modules"
- Désormais vos variables personnalisées dans "config.inc.php" doivent être dans "/personnalisation/configperso.inc.php" (fichier à créer vous-même, cela empèchera les prochaines mises à jour d'écraser vos modifications)

Vous devrez importer vos images via l'administration.

Licence
-------------
**GRR** est publié sous les termes de la **GNU General Public Licence**, dont le contenu est disponible dans le fichier "**LICENSE**", en anglais et dans le fichiers "**licence_fr.html**" en français. **GRR** est gratuit, vous pouvez le copier, le distribuer, et le modifier, à condition que chaque partie de **GRR** réutilisée ou modifiée reste sous licence **GNU GPL**. Par ailleurs et dans un soucis d'efficacité, merci de rester en contact avec le développeur de **GRR** pour éventuellement intégrer vos contributions à une distribution ultérieure.

Enfin, **GRR** est livré en l'état sans aucune garantie. Les auteurs de cet outil ne pourront en aucun cas être tenus pour responsables d'éventuels bugs.


Remarques concernant la sécurité
-------------------

La sécurisation de **GRR** est dépendante de celle du serveur. Nous vous recommandons d'utiliser un serveur Apache ou Nginx sous Linux, en utilisant le protocole **https** (transferts de données cryptées), et en veillant à toujours utiliser les dernières versions des logiciels impliqués (notamment **Apache/Nginx** et **PHP**).

L'EQUIPE DE DEVELOPPEMENT DE GRR NE SAURAIT EN AUCUN CAS ETRE TENUE POUR RESPONSABLE EN CAS D'INTRUSION EXTERIEURE LIEE A UNE FAIBLESSE DE GRR OU DE SON SUPPORT SERVEUR.

(*) en cas de dysfonctionnement, il est possible que d'autres modules de PHP soient manquants. Merci d'en tenir l'équipe de développement informée.
