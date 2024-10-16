## Documentation Administrateur de Security Onion

### SOMMAIRE
- [Licence de cette documentation](https://github.com/rikiya-gabimaru/Security-Onion-Start/blob/main/INSTALL.md#licence-de-cette-documentation)
- [Prérequis techniques](https://github.com/rikiya-gabimaru/Security-Onion-Start/blob/main/INSTALL.md#%C3%A9tapes-dinstallation-et-de-configuration-de-security-onion-24-)
- [Prérequis techniques](https://github.com/rikiya-gabimaru/Security-Onion-Start/blob/main/INSTALL.md#%C3%A9tapes-dinstallation-et-de-configuration-de-security-onion-24-)
- [Étapes d'installation et de configuration de Security Onion 2.4](https://github.com/rikiya-gabimaru/Security-Onion-Start/blob/main/INSTALL.md#%C3%A9tapes-dinstallation-et-de-configuration-de-security-onion-24-)
- [FAQ](https://github.com/rikiya-gabimaru/Security-Onion-Start/blob/main/INSTALL.md#faq-)

### Licence de cette documentation
- Cette documentation est sous licence [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/deed.fr)

### Prérequis techniques :

**Security Onion (Standalone) :**
  - CPU architecturex86-64 architecture (standard Intel or AMD 64-bit processors)
  - CPUs : 4
  - RAM : 16 GB
  - Storage : 200 GB (testé avec 100)
  - NICs : 2

### Étapes d'installation et de configuration de Security Onion 2.4 :

**1 - Téléchargement de l'ISO :**

   - [Accédez au téléchargement](https://docs.securityonion.net/en/2.4/download.html)

**2 - Vérifier l'intégrité de l'ISO :**

   - En BASH :
	```sha256sum securityonion-2.4.110-20241010.iso```
   - En CMD :
   	```certutil -hashfile securityonion-2.4.110-20241010.iso sha256```
   - En Powershell
	```Get-FileHash -Path "C:\ISO\securityonion-2.4.110-20241010.iso" -Algorithm SHA256```

**3 - Lancement de l'installation :**

   - Insérer l'ISO dans la machine
   - Booter sur l'ISO

**4 - Lors du premier écran de démarrage, sélectionner le premier choix.
><img src="https://github.com/WildCodeSchool/TSSR-2409-P1-G1-Plateforme-de-surveillance-de-securite/blob/main/Install_Screen_SecurityOnion/001.png?raw=true" alt="Pictures" width="300" height="300">

