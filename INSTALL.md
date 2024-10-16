## Documentation Administrateur de Security Onion

### I. SOMMAIRE
- [Licence de cette documentation](https://github.com/rikiya-gabimaru/Security-Onion-Start/blob/main/INSTALL.md#licence-de-cette-documentation)
- [Prérequis techniques](https://github.com/rikiya-gabimaru/Security-Onion-Start/blob/main/INSTALL.md#%C3%A9tapes-dinstallation-et-de-configuration-de-security-onion-24-)
- [Prérequis techniques](https://github.com/rikiya-gabimaru/Security-Onion-Start/blob/main/INSTALL.md#%C3%A9tapes-dinstallation-et-de-configuration-de-security-onion-24-)
- [Étapes d'installation et de configuration de Security Onion 2.4](https://github.com/rikiya-gabimaru/Security-Onion-Start/blob/main/INSTALL.md#%C3%A9tapes-dinstallation-et-de-configuration-de-security-onion-24-)
- [FAQ](https://github.com/rikiya-gabimaru/Security-Onion-Start/blob/main/INSTALL.md#faq-)

### II. Licence de cette documentation
- Cette documentation est sous licence [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/deed.fr)

### III. Prérequis techniques :

**Security Onion (Standalone) :**
  - CPU architecturex86-64 architecture (standard Intel or AMD 64-bit processors)
  - CPUs : 4
  - RAM : 16 GB
  - Storage : 200 GB (testé avec 100)
  - NICs : 2

### IV. Étapes d'installation et de configuration de Security Onion 2.4 :

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

**4 - Etapes d'installation**

4.1 - Lors de l'affichage du premier écran, sélectionner la première ligne  
>Sans choix de votre part, la première ligne est automatiquement choisi au bout du décompte.
<br><br>
<img src="https://github.com/WildCodeSchool/TSSR-2409-P1-G1-Plateforme-de-surveillance-de-securite/blob/main/Install_Screen_SecurityOnion/001.png?raw=true" alt="Pictures" width="800" >
<br><br>

4.2 - Taper `yes` lorsque cela vous est demander.
<br><br>
<img src="https://github.com/WildCodeSchool/TSSR-2409-P1-G1-Plateforme-de-surveillance-de-securite/blob/main/Install_Screen_SecurityOnion/002.png?raw=true" alt="Pictures" width="800" >
<br><br>

4.3 - Renseigner le nom d'utilisateur pour vous connecter à la console  
>Pour notre démo nous utiliserons `admin`
<br><br>
<img src="https://github.com/WildCodeSchool/TSSR-2409-P1-G1-Plateforme-de-surveillance-de-securite/blob/main/Install_Screen_SecurityOnion/003.png?raw=true" alt="Pictures" width="800" >
<br><br>

4.4 - Renseigner un mot de passe (attention clavier qwerty par défaut)
<br><br>
<img src="https://github.com/WildCodeSchool/TSSR-2409-P1-G1-Plateforme-de-surveillance-de-securite/blob/main/Install_Screen_SecurityOnion/004.png?raw=true" alt="Pictures" width="800" >
<br><br>

4.5 - Re-valider le mot de passe
<br><br>
<img src="https://github.com/WildCodeSchool/TSSR-2409-P1-G1-Plateforme-de-surveillance-de-securite/blob/main/Install_Screen_SecurityOnion/005.png?raw=true" alt="Pictures" width="800" >
<br><br>

4.6 - Après plusieurs ligne de défilement, cette écran vous invite à redémarrer en pressant `Entrée`
<br><br>
<img src="https://github.com/WildCodeSchool/TSSR-2409-P1-G1-Plateforme-de-surveillance-de-securite/blob/main/Install_Screen_SecurityOnion/006.png?raw=true" alt="Pictures" width="800" >
<br><br>

4.7 - A cet écran, taper le nom d'utilisateur rensigner à l'étape 4.3
<br><br>
<img src="https://github.com/WildCodeSchool/TSSR-2409-P1-G1-Plateforme-de-surveillance-de-securite/blob/main/Install_Screen_SecurityOnion/007.png?raw=true" alt="Pictures" width="800" >
<br><br>

4.8 - Puis votre mot de passe de l'étape 4.4
<br><br>
<img src="https://github.com/WildCodeSchool/TSSR-2409-P1-G1-Plateforme-de-surveillance-de-securite/blob/main/Install_Screen_SecurityOnion/008.png?raw=true" alt="Pictures" width="800" >
<br><br>

4.9 - Sélectionner `Yes` pour continuer
<br><br>
<img src="https://github.com/WildCodeSchool/TSSR-2409-P1-G1-Plateforme-de-surveillance-de-securite/blob/main/Install_Screen_SecurityOnion/009.png?raw=true" alt="Pictures" width="800" >
<br><br>

4.10 - Sélectionner `Install` puis `ok`
<br><br>
<img src="https://github.com/WildCodeSchool/TSSR-2409-P1-G1-Plateforme-de-surveillance-de-securite/blob/main/Install_Screen_SecurityOnion/010.png?raw=true" alt="Pictures" width="800" >
<br><br>


<br><br>
<img src="https://github.com/WildCodeSchool/TSSR-2409-P1-G1-Plateforme-de-surveillance-de-securite/blob/main/Install_Screen_SecurityOnion/011.png?raw=true" alt="Pictures" width="800" >
<br><br>


<br><br>
<img src="https://github.com/WildCodeSchool/TSSR-2409-P1-G1-Plateforme-de-surveillance-de-securite/blob/main/Install_Screen_SecurityOnion/012.png?raw=true" alt="Pictures" width="800" >
<br><br>


<br><br>
<img src="https://github.com/WildCodeSchool/TSSR-2409-P1-G1-Plateforme-de-surveillance-de-securite/blob/main/Install_Screen_SecurityOnion/013.png?raw=true" alt="Pictures" width="800" >
<br><br>


<br><br>
<img src="https://github.com/WildCodeSchool/TSSR-2409-P1-G1-Plateforme-de-surveillance-de-securite/blob/main/Install_Screen_SecurityOnion/014.png?raw=true" alt="Pictures" width="800" >
<br><br>


<br><br>
<img src="https://github.com/WildCodeSchool/TSSR-2409-P1-G1-Plateforme-de-surveillance-de-securite/blob/main/Install_Screen_SecurityOnion/015.png?raw=true" alt="Pictures" width="800" >
<br><br>


<br><br>
<img src="https://github.com/WildCodeSchool/TSSR-2409-P1-G1-Plateforme-de-surveillance-de-securite/blob/main/Install_Screen_SecurityOnion/016.png?raw=true" alt="Pictures" width="800" >
<br><br>


<br><br>
<img src="https://github.com/WildCodeSchool/TSSR-2409-P1-G1-Plateforme-de-surveillance-de-securite/blob/main/Install_Screen_SecurityOnion/017.png?raw=true" alt="Pictures" width="800" >
<br><br>


<br><br>
<img src="https://github.com/WildCodeSchool/TSSR-2409-P1-G1-Plateforme-de-surveillance-de-securite/blob/main/Install_Screen_SecurityOnion/018.png?raw=true" alt="Pictures" width="800" >
<br><br>


<br><br>
<img src="https://github.com/WildCodeSchool/TSSR-2409-P1-G1-Plateforme-de-surveillance-de-securite/blob/main/Install_Screen_SecurityOnion/019.png?raw=true" alt="Pictures" width="800" >
<br><br>


<br><br>
<img src="https://github.com/WildCodeSchool/TSSR-2409-P1-G1-Plateforme-de-surveillance-de-securite/blob/main/Install_Screen_SecurityOnion/020.png?raw=true" alt="Pictures" width="800" >
<br><br>


<br><br>
<img src="https://github.com/WildCodeSchool/TSSR-2409-P1-G1-Plateforme-de-surveillance-de-securite/blob/main/Install_Screen_SecurityOnion/021.png?raw=true" alt="Pictures" width="800" >
<br><br>


<br><br>
<img src="https://github.com/WildCodeSchool/TSSR-2409-P1-G1-Plateforme-de-surveillance-de-securite/blob/main/Install_Screen_SecurityOnion/022.png?raw=true" alt="Pictures" width="800" >
<br><br>


<br><br>
<img src="https://github.com/WildCodeSchool/TSSR-2409-P1-G1-Plateforme-de-surveillance-de-securite/blob/main/Install_Screen_SecurityOnion/023.png?raw=true" alt="Pictures" width="800" >
<br><br>


<br><br>
<img src="https://github.com/WildCodeSchool/TSSR-2409-P1-G1-Plateforme-de-surveillance-de-securite/blob/main/Install_Screen_SecurityOnion/024.png?raw=true" alt="Pictures" width="800" >
<br><br>


<br><br>
<img src="https://github.com/WildCodeSchool/TSSR-2409-P1-G1-Plateforme-de-surveillance-de-securite/blob/main/Install_Screen_SecurityOnion/025.png?raw=true" alt="Pictures" width="800" >
<br><br>


<br><br>
<img src="https://github.com/WildCodeSchool/TSSR-2409-P1-G1-Plateforme-de-surveillance-de-securite/blob/main/Install_Screen_SecurityOnion/026.png?raw=true" alt="Pictures" width="800" >
<br><br>


<br><br>
<img src="https://github.com/WildCodeSchool/TSSR-2409-P1-G1-Plateforme-de-surveillance-de-securite/blob/main/Install_Screen_SecurityOnion/027.png?raw=true" alt="Pictures" width="800" >
<br><br>


<br><br>
<img src="https://github.com/WildCodeSchool/TSSR-2409-P1-G1-Plateforme-de-surveillance-de-securite/blob/main/Install_Screen_SecurityOnion/028.png?raw=true" alt="Pictures" width="800" >
<br><br>


<br><br>
<img src="https://github.com/WildCodeSchool/TSSR-2409-P1-G1-Plateforme-de-surveillance-de-securite/blob/main/Install_Screen_SecurityOnion/029.png?raw=true" alt="Pictures" width="800" >
<br><br>


<br><br>
<img src="https://github.com/WildCodeSchool/TSSR-2409-P1-G1-Plateforme-de-surveillance-de-securite/blob/main/Install_Screen_SecurityOnion/030.png?raw=true" alt="Pictures" width="800" >
<br><br>


<br><br>
<img src="https://github.com/WildCodeSchool/TSSR-2409-P1-G1-Plateforme-de-surveillance-de-securite/blob/main/Install_Screen_SecurityOnion/031.png?raw=true" alt="Pictures" width="800" >
<br><br>


<br><br>
<img src="https://github.com/WildCodeSchool/TSSR-2409-P1-G1-Plateforme-de-surveillance-de-securite/blob/main/Install_Screen_SecurityOnion/032.png?raw=true" alt="Pictures" width="800" >
<br><br>


<br><br>
<img src="https://github.com/WildCodeSchool/TSSR-2409-P1-G1-Plateforme-de-surveillance-de-securite/blob/main/Install_Screen_SecurityOnion/033.png?raw=true" alt="Pictures" width="800" >
<br><br>


<br><br>
<img src="https://github.com/WildCodeSchool/TSSR-2409-P1-G1-Plateforme-de-surveillance-de-securite/blob/main/Install_Screen_SecurityOnion/034.png?raw=true" alt="Pictures" width="800" >
<br><br>


<br><br>
<img src="https://github.com/WildCodeSchool/TSSR-2409-P1-G1-Plateforme-de-surveillance-de-securite/blob/main/Install_Screen_SecurityOnion/035.png?raw=true" alt="Pictures" width="800" >
<br><br>


<br><br>
<img src="https://github.com/WildCodeSchool/TSSR-2409-P1-G1-Plateforme-de-surveillance-de-securite/blob/main/Install_Screen_SecurityOnion/036.png?raw=true" alt="Pictures" width="800" >
<br><br>


<br><br>
<img src="https://github.com/WildCodeSchool/TSSR-2409-P1-G1-Plateforme-de-surveillance-de-securite/blob/main/Install_Screen_SecurityOnion/037.png?raw=true" alt="Pictures" width="800" >
<br><br>




