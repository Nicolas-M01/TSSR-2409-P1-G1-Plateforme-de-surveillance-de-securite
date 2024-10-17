# Documentation Utilisateur
---
## Sommaire

1) [Définition Security Onion : SIEM](https://github.com/WildCodeSchool/TSSR-2409-P1-G1-Plateforme-de-surveillance-de-securite/edit/main/USER_GUIDE.md#definition-security-onion)
2) [Utilisation de Base](https://github.com/WildCodeSchool/TSSR-2409-P1-G1-Plateforme-de-surveillance-de-securite/edit/main/USER_GUIDE.md#utilisation-de-Base)
4) [Utilisation avancée](https://github.com/WildCodeSchool/TSSR-2409-P1-G1-Plateforme-de-surveillance-de-securite/edit/main/USER_GUIDE.md#utilisation-avancee)
5) [FAQ : solutions aux problèmes connus et communs liés à l’utilisation](https://github.com/WildCodeSchool/TSSR-2409-P1-G1-Plateforme-de-surveillance-de-securite/edit/main/USER_GUIDE.md#faq-:-solutions-aux-problemes-connus-et-communs-lies-a-l-utilisation)
  


## :one: Définition Security Onion
Security Onion est un SIEM : Système de gestion des événements et des informations de sécurité. C'est un système centralisé qui permet une visibilité globale sur l'ensemble de l'activité du réseau et qui permet de régir aux menaces.
Security Onion est une distribution Linux (basée sur Fedora) open source conçue pour la surveillance et l'analyse de la sécurité réseau. Elle est spécifiquement développée pour aider les organisations à détecter et à répondre aux menaces de sécurité en fournissant des outils puissants pour la surveillance du trafic réseau, l'analyse des journaux et la détection d'intrusions.  


## :two: Utilisation de base
### Connexion
Une fois l'installation terminée, connectez vous avec l'adresse IP de votre installation Security Onion. Connectez vous à l'aide de l'adresse mail et mot de passe spécifiés pendant l'installation.

![écran login](https://docs.securityonion.net/en/2.4/_images/37_login.png)  

  
Une fois connecté, vous remarquerez le menu principal sur la partie gauche avec les liens vers des outils d'analyste tels que Alerts, Dashboards, Hunts, Cases, Detections, PCAP, Kibana, CyberChef et ATT&CK Navigator. Le menu utilisateur est en haut à droite pour accéder à la doc et autres ressources et gérer les paramètres utilisateur.

![UserMenu](https://docs.securityonion.net/en/2.4/_images/94_usermenu.png)

### Alerts 
Security Onion comprend une interface Alertes qui vous donne un aperçu des alertes générées par Security Onion. Vous pouvez ensuite accéder rapidement aux détails, basculer vers Hunt ou l'interface PCAP et faire remonter les alertes vers les dossiers .

![Alerts](https://docs.securityonion.net/en/2.4/_images/50_alerts.png)


### Dashboards
Security Onion comprend une interface de tableaux de bord qui comprend un ensemble complet de tableaux de bord prédéfinis. Les informations sont paramétrables, comme l'intervalle de rafraichissement et l'inclusion/exclusion de certaines informations.

![Dashboards](https://docs.securityonion.net/en/2.4/_images/53_dashboards.png)

### Hunt
Il comprend également une interface proche de Dashboards. Mais dans Hunt les rêquetes sont plus ciblées que dans Dashboards et il est plutôt adapté à la recherche de menace.

![Hunt](https://docs.securityonion.net/en/2.4/_images/56_hunt.png)


### Cases
Cette interface est utilisée pour la gestion des cas. Elle permet de faire remonter les journaux de Alerts, Dashboards et Hunt. Elle permet ensuite d'affecter des analystes, de rajouter des commentaires et des pièces jointes et de suivre ce qui est observable.

![Cases](https://docs.securityonion.net/en/2.4/_images/57_0_cases.png)


### Detection
Cette interface sert à paramétrer les règles de détection pour gérer les règles.

![Detection](https://docs.securityonion.net/en/2.4/_images/57_detections.png)


### PCAP
PCAP permet d'accéder aux captures de paquets du réseau, qui ont été écrites pas Suricata par exemple.

![PCAP](https://docs.securityonion.net/en/2.4/_images/62_pcap.png)


### Grid
Cette interface permet de voir l'état des noeuds du réseau.

![Grid](https://docs.securityonion.net/en/2.4/_images/39_grid.png)


### Downloads
Cette interface permet de télécharger ElasticAgent

![Downloads](https://docs.securityonion.net/en/2.4/_images/78_downloads.png)


### Administration
La partie administration permet de gérer les utilisateurs, les membres du réseau, la confirguration et la clé de licence.

![Adminnistration](https://docs.securityonion.net/en/2.4/_images/81_users.png)


## :three: Utilisation avancée
  * #### Surveillance du traffic réseau
    Security Onion utilise des outils tels que **Suricata** et **Zeek**.
    
    >***Suricata :*** Cet outil va analyser le traffic sur une ou plusieurs interfaces réseaux en temps réel en fonction des règles activées. Il génère un fichier qui peut     
    ensuite être utilisé par Logstash ou ElasticSearch. Outil puissant pour la détection et prévention d'intrusion.
    
    >***Zeek :*** Cet outil est également un analyseur de traffic réseau, mais plus passif que Suricata. Il capture et analyse les paquets pour une utilisation ultérieur.
    
    
  * #### Analyse de journaux
    Il intègre des outils comme **ElasticSearch**, **Logstash** et **Kibana** appelés suite "ELK". Cette suite de logiciels permet de collecter n'importe quel format de données depuis n'importe quelle source pour les analyser.
    
    >***ElasticSearch :*** Moteur de recherche et d'analyse, il centralise le stockage de vos données et fournit une recherche rapide et pertinante. Choix idéal dans l'analyse des journaux. Il indexe, analyse et recherche les données ingéres.
    
    >***Logstash :*** Permet de collecter les données de diverses sources, de les transformer et de les envoyer. Il sert souvent de "pipeline" côté serveur, pour envoyer vers        ElasticSearch. Il ingère, transforme et les données à bonne destination.

    >***Kibana :*** Outil de visualisation des journaux analysés. Il propose différentes formes de graphiques et de rapports intuitifs utilisés pour naviguer de manière interactive dans de grandes quantités de données. Il visualise les résultats.

    
  
  * #### HoneyPots de détection d'intrusion
    Security Onion dispose d'un noeud HoneyPot qui imite les services, basé sur **OpenCanary**. Toute intrusion à ces services génère automatiquement une alerte.

    >***OpenCanary :*** Capable de simuler plusieurs services et applications susceptibles d'être ciblés par des attaquants tels que des serveurs SSH, HTTP, FTP...

## :four: FAQ : solutions aux problèmes connus et communs liés à l’utilisation
