# TSSR-2409-P1-G1-Plateforme-de-surveillance-de-securite#
  ### Présentation du projet: 

 - Le projet consiste à présenter un serveur ( Security Onion ) qui sécurisera le client

  ### objectif finale:

 - Bénéficiez d'une visibilité complète sur le réseau et le client afin de détecter toutes intrusions grâce aux outils d’analyse  ( en cours ) 

 ### Introduction : mise en contexte

- Création du serveur Security Onion

- Création du ou des clients 

- Sécurisation du Client
#
- La sécurisation du client grâce au serveur est essentielle car il gère des informations sensibles telles que les données utilisateur, la logique métier et les communications avec les bases de données et les API.( Interfaces de Programmation d'Applications ) ou ensembles de règles et de protocoles qui permettent à différentes applications ou systèmes de communiquer entre eux.


### Membres du groupe de projet (rôles par sprint):

      -Scrum Master > Nicolas

        - Product Owner > Freddy

           -Collaborateurs > William et François



 ### Choix techniques : quel OS, quelle version, etc.:
 #
 #


### Os d'installation:

- Security Onion 2.4.110 tourne sur la distribution Fedora Linux. Pour une installation en standalone nécessitant 4 coeurs, 16Go de Ram et 100Go d'espace disque.


### Difficultés rencontrées : problèmes techniques rencontrés
#
#

### Limitations matériels:

- Le premier obstacle évident se situe au niveau d'une config relativement robuste pour pouvoir faire tourner décemment une version standalone.
Les options plus légères n'ont pas abouti aux résultats escomptés.

### Configuration réseau:

- La configuration réseau nécessite d'anticiper si l'on souhaite établir une communication avec l'hôte, nécessitant une connexion par pont.
Ou s'il est préférable de faire communiquer VM clients et serveur entre eux grace à une connexion NAT.
Ces choix devraient se faire en fonction des potentialités futures (de quelles fonctionnalités aurons- nous besoin, la facilitation de leur usage peut dépendre du type de réseau).
La difficulté à notre étape consiste à essayer d'anticiper ce que nous ne connaissons ni ne maîtrisons pas encore bien.


### Solutions trouvées : Solutions et alternatives trouvées 
#
#

### Solution matériel:

- Nous avons opté pour un support d'installation ***proxmox*** (?)

### Solution configuration réseau:

- Bien que sans doute moins sécurisé pour la machine hôte (en cas de tests), nous avons opté pour l'accès par pont qui semblait avoir une configuration plus flexible dans l'installation.


## Améliorations possibles : suggestions d'améliorations futures


