# Publication de 360-design.fr

Ce dépôt ne contient pas de code. Il sert uniquement de point de
téléchargement public pour l'hébergement o2switch du site
[360-design.fr](https://360-design.fr).

La release **`publication`** porte, remplacés à chaque mise à jour :

| Fichier | Contenu |
|---|---|
| `site-<commit>.zip` | le site compilé, c'est-à-dire exactement ce que le site sert déjà en ligne |
| `version.json` | identifiant du commit, horodatage, taille, nombre de fichiers, empreinte SHA-256 de l'archive |
| `synchroniser-site.php` | le script que le serveur d'o2switch exécute en tâche planifiée |

Le serveur lit `version.json`, s'arrête si la version installée est déjà la
bonne, sinon télécharge l'archive, vérifie son empreinte et l'installe.

Aucun code source, aucun secret, aucun contenu privé n'est publié ici.
