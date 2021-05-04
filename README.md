# mysql-16gb-config

## C'est quoi ?
Un exemple de configuration pour un serveur PHP7.3 + MySQL ayant 16gb de RAM à se répartir pour faire tourner des sites exécutant beaucoup de requêtes SQL assez lourdes.


## Est-ce qu'il faut configurer autre chose ?
Oui, il faut penser à augmenter la limite de la variable "open_files" à 65535 sous peine de brider les performances de MySQL. Vous pouvez obtenir cette limite via la commande : `ulimit -n`
