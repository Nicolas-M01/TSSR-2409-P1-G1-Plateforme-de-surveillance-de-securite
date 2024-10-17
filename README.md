# TSSR-2409-P1-G1-Plateforme-de-surveillance-de-securite
 <br><br>

SOMMAIRE

1. [Présentation du projet](#i-présentation-du-projet)
2. [Objectif final](#ii-objectif-final)
3. [Introduction : mise en contexte](#iii-introduction--mise-en-contexte)
4. [Membres du groupe de projet (rôles par sprint)](#iv-membres-du-groupe-de-projet-rôles-par-sprint)
5. [Choix techniques](#v-choix-techniques)
6. [Difficultés rencontrées](#vi-difficultés-rencontrées)
7. [Solutions trouvées et/ou alternatives](#vii-solutions-trouvées-etou-alternatives)
8. [Améliorations possibles : suggestions d'améliorations futures](#viii-améliorations-possibles--suggestions-daméliorations-futures)

<br><br>

  ## I. Présentation du projet: 

 - Le projet consiste à présenter un serveur ( Security Onion ) qui sécurisera le client

  ## II. Objectif final:

 - Bénéficiez d'une visibilité complète sur le réseau et le client afin de détecter toutes intrusions grâce aux outils d’analyse  ( en cours ) 

 ## III. Introduction : mise en contexte

- Création du serveur Security Onion

- Création du ou des clients 

- Sécurisation du Client
#
- La sécurisation du client grâce au serveur est essentielle car il gère des informations sensibles telles que les données utilisateur, la logique métier et les communications avec les bases de données et les API.( Interfaces de Programmation d'Applications ) ou ensembles de règles et de protocoles qui permettent à différentes applications ou systèmes de communiquer entre eux.


## IV. Membres du groupe de projet (rôles par sprint):

      -Scrum Master > Nicolas

        - Product Owner > Freddy

           -Collaborateurs > William et François


## V. Choix techniques
 
### Os d'installation

* Le SIEM Security Onion 2.4.110 repose sur la distribution Fedora Linux.
* Allocation de ressources pour une installation en standalone:
  * Architecture x86-64 / standard Intel ou processeur AMD 64-bit
  * 4 coeurs
  * 16Go de Ram
  * minimum 100Go d'espace disque (200Go officiellement).
  * 2 cartes réseau
 
  * 
Étapes d'installation et de configuration de Security Onion 2.4 :

1 - Téléchargement de l'ISO :

https://docs.securityonion.net/en/2.4/download.html

2 - Vérifier l'intégrité de l'ISO :

En BASH : sha256sum securityonion-2.4.110-20241010.iso
En CMD : certutil -hashfile securityonion-2.4.110-20241010.iso sha256
En Powershell Get-FileHash -Path "C:\ISO\securityonion-2.4.110-20241010.iso" -Algorithm SHA256

3 - Lancement de l'installation initiale :

Insérer l'ISO dans la machine
Booter sur l'ISO
Sélectionner "Install Security Onion 2.4.110"
Configurer un nom d'administrateur et un mot de passe
Redémarrer la machine à la fin de l'installation initiale

4 - Installation standard et configuration :

Au redémarrage de la machine, choisir "Yes" pour commencer la configuration
Lancer l'installation standard de Security Onion
Sélectionner "Standard" afin de permettre au gestionnaire d'installation d'avoir accès à Internet
Sélectionner le type d'installation souhaité (dans notre cas STANDALONE)
Accepter la licence en tapant "AGREE"
Entrer un nom pour votre plateforme Security Onion
Choisir l'interface réseau par laquelle la gestion admin sera effectuée
Choisir le type d'adressage pour cette interface réseau (statique ou DHCP)
Affecter une adresse statique pour l'interface de gestion admin (si choix de l'adressage statique)
Entrer l'adresse de la passerelle du réseau
Entrer l'adresse des serveurs DNS
Entrer un nom de domaine
Valider les informations de réseau précédemment
Sélectionner la manière de se connecter à Internet
Entrer une adresse web afin de permettre la connexion à l'interface web de gestion admin
Définir un mot de passe pour la WUI puis confirmer son mot de passe
Définir par quel moyen se connecter à la WUI (IP, HOSTNAME, OTHER)
Autoriser l'accès via la WUI
Définir l'IP ou les réseaux de confiances qui pourront gérer Security Onion par la WUI
Définir l'activation ou non de la télémétrie pour aider l'équipe de développement du projet
Valider le résumé de la configuration

5 - Fin de configuration :

Valider la fenêtre de fin de configuration

FAQ :

- En cours de construction...


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
