# BiblioMax : versions signées

Ce dépôt ne contient ni le code ni les installateurs de BiblioMax. Il publie seulement, pour chaque
version proposée aux testeurs, une petite fiche signée :

- `derniere-version.json` : numéro de version, taille et empreinte SHA-256 de l'installateur ;
- `derniere-version.json.sig` : sa signature (RSA-3072, SHA-256).

Les PC des testeurs lisent la fiche de la dernière version (onglet Releases). Ils n'installent un
fichier que si la signature est faite par l'une des clés inscrites dans BiblioMax et si le fichier
a exactement l'empreinte annoncée. L'installateur lui-même se télécharge dans un dépôt privé, avec
la clé personnelle de chaque testeur.

Une fiche n'est signée qu'après l'approbation du responsable (environnement « signature »).
