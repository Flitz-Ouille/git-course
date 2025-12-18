Prendre en main Git et GitHub : création de dépôt, gestion de branches, commits, merges et travail avec une connexion SSH.



Installation de Git (exemple Windows) :



https://git-scm.com/download/win



Puis vérifier la version :

git --version



------



\- Documentation officielle Git : https://git-scm.com/doc  

\- Référence des commandes Git : https://git-scm.com/docs/git  

\- Documentation GitHub sur l’utilisation de Git : https://docs.github.com/en/get-started/using-git/about-git  



Commandes réalisées :



| Commande                                   | Description                                                        |

|-------------------------------------------|--------------------------------------------------------------------|

| `git --version`                           | Vérifier que Git est installé.                                    |

| `git config --global user.name`           | Définir le nom de l’utilisateur pour les commits.                 |

| `git config --global user.email`          | Définir l’email de l’utilisateur pour les commits.                |

| `ssh-keygen -t ed25519 -C "email"`        | Générer une clé SSH pour GitHub.                                  |

| `git clone git@github.com:.../git-course.git` | Cloner le dépôt distant en local.                           |

| `git checkout -b develop`                 | Créer et basculer sur la branche `develop`.                       |

| `touch file1 file2 file3`                 | Créer les fichiers dans le dossier `DevOps`.                      |

| `git add ...`                             | Ajouter les fichiers au prochain commit.                          |

| `git commit -m "message"`                 | Enregistrer les modifications dans l’historique local.            |

| `git push -u origin develop`              | Pousser la branche `develop` vers GitHub.                         |

| `git checkout -b main` / `git checkout main` | Créer ou basculer sur la branche `main`.                     |

| `git merge develop`                       | Fusionner les changements de `develop` dans la branche courante.  |

| `mv DevOps/file1 DevOps/file1.txt`        | Renommer `file1` en `file1.txt`.                                  |

| `rm DevOps/file3`                         | Supprimer le fichier `file3`.                                     |





Diagramme textuel simplifié du flux réalisé pendant le TP :



Création dépôt GitHub (git-course)

|

v

git clone (branche main locale)

|

v

git checkout -b develop

|

v

Ajout file1, file2, file3 dans DevOps

git add / git commit / git push (develop)

|

v

git checkout -b main (main = develop)

|

v

git checkout develop



création et mise à jour du README



renommage file1 -> file1.txt



suppression file3

git add / git commit / git push (develop)

|

v

git checkout main

git merge develop

git push (main à jour avec develop)



undefined


Lucas LESENS




