# Cheatsheet

Cette petite fiche regroupe toutes les commandes git utilisées dans la mise en situation (et en ajoute quelques unes). A utiliser en cas d'oubli !



| Commande                                              | Description                                                                                                                                                       |
|:-----------------------------------------------------:|:-----------------------------------------------------------------------------------------------------------------------------------------------------------------:|
| `git init`                                            | Fait du dossier courant un repository git.                                                                                                                        |
| `git clone $REPOSITORY_URL`                           | Clone le repository dont l'URL est donné en argument dans le dossier où la commande est utilisée.                                                                 |
| `git branch`                                          | Liste les branches existantes en local.                                                                                                                           |
| `git fetch`                                           | Récupère la liste des changements existants en remote. Ne remplace rien de ce qui existe en local, mais permet de comparer ce qui existe en local avec la remote. |
| `git pull`                                            | Récupère les changements en de la branche courante remote et tente de les merger dans la branche locale.                                                          |
| `git log`                                             | Affiche l'historique des commits de la branche courante.                                                                                                          |
| `git status`                                          | Liste les changements effectués et leur statut. Si des opérations de rebase ou de merge sont en cours, affiche leur état.                                         |
| `git checkout $BRANCH_NAME`                           | Permet de se positionner sur la branche spécifiée.                                                                                                                |
| `git checkout -b $NEW_BRANCH_NAME`                    | Crée une branche avec le nom spécifiée et se déplace dessus.                                                                                                      |
| `git branch -m`                                       | Renomme la branche courante.                                                                                                                                      |
| `git reset --hard`                                    | Détruit tous les changements effectués depuis le dernier commit.                                                                                                  |
| `git add $FILE`                                       | Ajoute le fichier spécifié aux changements à committer.                                                                                                           |
| `git add .`                                           | Ajoute tous les changements aux changements à committer.                                                                                                          |
| `git commit -m $COMMIT_MESSAGE`                       | Committe les changements avec le message spécifié.                                                                                                                |
| `git push (--set-upstream $REMOTE_NAME $BRANCH_NAME)` | Pushe les changements sur la branche en remote. L'argument `-f` permet de forcer le push s'il y a des conflits d'historique.                                      |
| `git rebase $TARGET_BRANCH`                           | Place l'origine de la branche courante à la fin de la branche cible.                                                                                              |
| `git rebase -i HEAD~$NUMBER`                          | Rebase interactivement la branche en cours pour éditer le nombre de commits voulu.                                                                                |
| `git stash`                                           | Met de côté les changements en cours.                                                                                                                             |
| `git stash pop`                                       | Applique et oublie les changements mis de côté.                                                                                                                   |
| `git cherry-pick $COMMIT_ID`                          | Récupère le commit spécifié et le place en tête de la branche courante.                                                                                           |

