## Master 1 SDL/IHM - UE MAAR - Introduction à RMI

### LAST NAME :
### First name :
### TP group :
- [ ] 41
- [ ] 42
- [ ] 51
- [ ] 52

### Préliminaire

1. Mettez dans vos favoris le lien vers la [documentation de RMI](https://docs.oracle.com/javase/8/docs/technotes/guides/rmi/).
2. Clonez ce dépôt GitHub en ligne de commande et importez le comme projet Maven dans IntelliJ :
   <kbd>File → New → Project-from-Existing-Sources…</kbd>.

### Partie 1 - Hello World (travail individuel)

Oracle met à disposition un [guide de démarrage avec RMI](https://docs.oracle.com/javase/8/docs/technotes/guides/rmi/hello/hello-world.html).
Étudiez et implantez dans votre projet l'exemple proposé par ce guide de démarrage.
Vérifiez en lançant les différents composants de l'architecture distribuée que tout fonctionne comme attendu.
En cas de problème au lancement du serveur, ce lien peut-être utile : http://docs.oracle.com/javase/7/docs/technotes/guides/rmi/enhancements-7.html

### Partie 2 - LightSlack (travail en binôme)

L'objectif de cette activité est le développement d'un serveur et d'un client de discussion (très) rudimentaire.

1. Pour travailler en binôme, vous pouvez choisir de travailler dans un de vos deux dépôts, après avoir ajouté votre binôme comme collaborateur : <kbd>Settings → Collaborators and teams</kbd> (pour ce TP GitHub Classroom, vous avez normalement les droits d'administration sur votre dépôt privé).
2. Implantez un serveur de discussion en mode synchrone exposant ses opérations clés via RMI.
3. Implantez un client RMI de votre serveur de discussion en utilisant les librairies d'interface de votre choix (JavaFX, Swing, ligne de commande).
 
### Aide pour lancer RMI

Lancer le serveur RMI:
```
rmiregistry -J-Djava.rmi.server.codebase=file:/{Project-Path}/m2-pcr-rmi-etu/target/classes/
```

Lancer un main:
Ajouter dans la configuration d'Intellij, dans VM Options
```
-Djava.rmi.server.codebase=file:/{Project-Path}/m2-pcr-rmi-etu/target/classes/
```
