# Exercice 1. Variables d’environnement

1. Dans quels dossiers bash trouve-t-il les commandes tapées par l’utilisateur ?
 (which ls)
 
2. Quelle variable d’environnement permet à la commande cd tapée sans argument de vous ramener dans
votre répertoire personnel ? Elle prend la valeur situé dans la variable environnement HOME.
(printenv HOME)

3. Explicitez le rôle des variables LANG, PWD, OLDPWD, SHELL et _.
 * la variable LANG  : Détermine la langue que les logiciels utilisent pour communiquer avec l’utilisateur.
 *  PWD : Afiche le repertoire courant dans le quel on se situe
 * OLDPWD: Contient le chemin absolu vers le répertoire courant précédent (permet de savoir d'où on vient).
 * SHELL : L'interpréteur de commande préféré de l'utilisateur tel qu'il est défini dans le fichier « /etc/passwd ».
 * _ : Chemin de la dernière commande tapée dans le prompt.
 
4. Créez une variable locale MY_VAR (le contenu n’a pas d’importance). Vérifiez que la variable existe.
 Pour créer une variable environnement, on peut utiliser les commandes (export) ou (declare -x).
 On ecrit donc export MY_VAR="123456789" et on peut vérifier son contenu avec un printenv et son existence grâce à la commande (env) qui  liste les variables d'environnement présente.
5.Tapez ensuite la commande bash. Que fait-elle ? La variable MY_VAR existe-t-elle ? Expliquez. A la fin
de cette question, tapez la commande exit pour revenir dans votre session initiale.
la commande (bash.) supprime la variable local crée 

6. Transformez MY_VAR en une variable d’environnement et recommencez la question précédente. Expliquez.
 Meme apres la commande (bash ) la variable crée existe car un variable d'environnement pas local.
 
7. Créer la variable d’environnement NOMS ayant pour contenu vos noms de binômes séparés par un espace.
Afficher la valeur de NOMS pour vérifier que l’affectation est correcte.

* (EXPORT NOM=" PEROT KABA) créé la variable
* (printenv NOM) affiche le contenu

8. Ecrivez une commande qui affiche ”Bonjour à vous deux, binôme1 binôme2 !” (où binôme1 et binôme2
sont vos deux noms) en utilisant la variable NOMS.
 * (echo "bonjour , $NOM") 

9. Quelle différence y a-t-il entre donner une valeur vide à une variable et l’utilisation de la commande
unset ?
unset : Supprime la varible d'environnement alors que dans l'autre cas c'est juste le contenu qui est vide mais existe 

10.  Utilisez la commande echo pour écrire exactement la phrase : $HOME = chemin (où chemin est votre
dossier personnel d’après bash)
 (echo -e \$HOME= $HOME)
  # Programmation Bash
   * Ajoutez le chemin vers script à votre PATH de manière permanente.
  # Exercice 2. Contrôle de mot de passe
  
   
   
   


