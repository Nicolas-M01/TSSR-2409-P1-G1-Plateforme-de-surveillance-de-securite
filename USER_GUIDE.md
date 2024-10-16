# Documentation Utilisateur
---
## Sommaire

1) [Définition Security Onion : SIEM](#SIEM)
2) [Utilisation de Base](#Utilisation-de-Base)
4) [Utilisation avancée](#Utilisation-avancée)
5) [FAQ : solutions aux problèmes connus et communs liés à l’utilisation](#FAQ)


## 1) Définition Security Onion
Security Onion est une distribution Linux open source conçue pour la surveillance et l'analyse de la sécurité réseau. Elle est spécifiquement développée pour aider les organisations à détecter et à répondre aux menaces de sécurité en fournissant des outils puissants pour la surveillance du trafic réseau, l'analyse des journaux et la détection d'intrusions.


## 2) Utilisation de Base
### Connexion
Une fois l'installation terminée, connectez vous avec l'adresse IP de votre installation Security Onion. Connectez vous à l'aide de l'adresse mail et mot de passe spécifiés pendant l'installation.

![écran login](https://docs.securityonion.net/en/2.4/_images/37_login.png)  

  
Une fois connecté, vous remarquerez le menu principal sur la partie gauche avec les liens vers des outils d'analyste tels que Alerts, Dashboards, Hunts, Cases, Detections, PCAP, Kibana, CyberChef et ATT&CK Navigator. Le menu utilisateur est en haut à droite pour accéder à la doc et autres ressources et gérer les paramètres utilisateur.

![UserMenu](https://docs.securityonion.net/en/2.4/_images/94_usermenu.png)

### Alertes 
Security Onion comprend une interface Alertes qui vous donne un aperçu des alertes générées par Security Onion. Vous pouvez ensuite accéder rapidement aux détails, basculer vers Hunt ou l'interface PCAP et faire remonter les alertes vers les dossiers .

![Alerts](https://docs.securityonion.net/en/2.4/_images/50_alerts.png)


### Dashboards
Security Onion comprend une interface de tableaux de bord qui comprend un ensemble complet de tableaux de bord prédéfinis. Les informations sont paramétrables, comme l'intervalle de rafraichissement et l'inclusion/exclusion de certaines informations.

![Dashboards](https://docs.securityonion.net/en/2.4/_images/53_dashboards.png)

### Hunt
### Cases
### Detection
### PCAP
### Grid
### Downloads
### Administration





## 3) Utilisation avancée
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

## 4) FAQ : solutions aux problèmes connus et communs liés à l’utilisation
