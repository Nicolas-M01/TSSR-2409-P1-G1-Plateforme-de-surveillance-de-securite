# TSSR-2409-P1-G1-Plateforme-de-surveillance-de-security Onion
 <br><br>

SOMMAIRE

1. [Présentation du projet](#i-présentation-du-projet)
2. [Objectif final](#ii-objectif-final)
3. [Introduction : mise en contexte](#iii-introduction--mise-en-contexte)
4. [Membres du groupe de projet (rôles par sprint)](#iv-membres-du-groupe-de-projet-rôles-par-sprint)
5. [Choix techniques](#-choix-technique)
6. [Difficultés rencontrées](#vi-difficultés-rencontrées)
7. [Solutions trouvées et/ou alternatives](#vii-solutions-trouvées-etou-alternatives)
8. [Améliorations possibles : suggestions d'améliorations futures](#viii-améliorations-possibles--suggestions-daméliorations-futures)

<br><br>

  ## I. Présentation du projet: 

 - Le projet consiste à présenter un serveur ( Security Onion ) qui sécurisera le client

  ## II. Objectif final:

 - Bénéficiez d'une visibilité complète sur le réseau et le client afin de détecter toutes intrusions grâce aux outils d’analyse  ( en cours ) 

 ## III. Introduction : mise en contexte

- Création du serveur Security Onion et d'un agent

- Création du ou des clients 

- Sécurisation du Client
#
- La sécurisation du client grâce au serveur est essentielle car il gère des informations sensibles telles que les données utilisateur, la logique métier et les communications avec les bases de données et les API.( Interfaces de Programmation d'Applications ) ou ensembles de règles et de protocoles qui permettent à différentes applications ou systèmes de communiquer entre eux.


## IV. Membres du groupe de projet (rôles par sprint):

      -Scrum Master > Nicolas

        - Product Owner > Freddy

           -Collaborateurs > William et François


## V. Choix techniques
 


## VI. Difficultés rencontrées


### Limitations matérielles

Le premier obstacle se situe au niveau d'allocation de ressources nécessaires pour la stabilité du SIEM.
La version standalone, privilégiée pour bénéficier d'une solution complète, ne peut s'installer sur des configurations standards (de 16Go Ram et inférieur).
Des tests de versionns plus légères n'ont pas abouti aux résultats escomptés.
Généralement l'installation nous notifie d'une allocation de ressources trop faible.

### Configuration réseau

La configuration réseau a besoin d'être anticipée. Le parcours de l'installation propose plusieurs types de connexions.
Cependant les options à venir en dépendent et ces étapes déterminent la flexibilité avec laquelle peut s'établir la connexion à l'hôte.
De même, c'est à cette étape qu'il est préférable de savoir quels types de machines seront présentes sur le réseau, machines virtuelles ou non et si VM, connexion à la machine hôte ou non.

## VII. Solutions trouvées et/ou alternatives  

### Solution matérielle

Nous avons opté pour un support d'installation et virtualisation par ***proxmox*** (?)

### Solution configuration réseau

Après plusieurs essais et type de connexions, l'accès par pont semble permettre plus de flexibilité à l'installation et nous a permis de tester la connexion au serveur.

## VIII. Améliorations possibles : suggestions d'améliorations futures

D'autres pistes de configurations réseau ou d'environnements de test seront envisagées lorsque la solution sera plus amplement comprise et stable.
