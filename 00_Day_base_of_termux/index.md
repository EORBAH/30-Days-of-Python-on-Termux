
**Les bases de Termux de A à Z**

### 1. Introduction à Termux  

#### 1.1 Qu'est-ce que Termux ?  
Termux est un émulateur de terminal pour Android qui fournit un environnement Linux complet.  
Il permet d’exécuter des commandes Unix/Linux, d’écrire des scripts, d’installer des paquets, et même de coder en Python, C, ou d’autres langages.  

#### 1.2 Installation de Termux  
- Télécharger Termux depuis **F-Droid** (recommandé) ou via le site officiel.  
- **NE PAS** utiliser la version du Play Store, qui n’est plus mise à jour.  

#### 1.3 Premiers pas dans Termux  
Lancer Termux et entrer la commande :  
```bash
echo "Bienvenue dans Termux !"
```  
- Comprendre l'affichage et la structure des fichiers dans `$HOME`.  
- Exécuter les commandes de base :  
  ```bash
  pwd     # Affiche le répertoire actuel
  ls      # Liste les fichiers et dossiers
  cd      # Change de dossier
  mkdir   # Crée un nouveau dossier
  rm      # Supprime un fichier
  ```  

---  

### 2. Gestion des paquets et mises à jour  

#### 2.1 Mise à jour de Termux  
Avant d’installer quoi que ce soit, toujours mettre à jour Termux :  
```bash
pkg update && pkg upgrade
```  

#### 2.2 Installer et supprimer des paquets  
- Installer un package (ex: Python) :  
  ```bash
  pkg install python
  ```  
- Désinstaller un package :  
  ```bash
  pkg uninstall python
  ```  

#### 2.3 Rechercher des paquets  
- Voir les paquets disponibles :  
  ```bash
  pkg list-all
  ```  
- Rechercher un paquet spécifique :  
  ```bash
  pkg search nano
  ```  

---  

### 3. Gestion des fichiers et permissions  

#### 3.1 Commandes de base  
- Créer un fichier et un dossier :  
  ```bash
  touch fichier.txt
  mkdir mon_dossier
  ```  
- Copier et déplacer un fichier :  
  ```bash
  cp fichier.txt mon_dossier/
  mv fichier.txt mon_dossier/
  ```  
- Supprimer un fichier/dossier :  
  ```bash
  rm fichier.txt
  rm -rf mon_dossier
  ```  

#### 3.2 Modifier un fichier avec un éditeur  
- Installer nano et modifier un fichier :  
  ```bash
  pkg install nano
  nano fichier.txt
  ```  
  Sauvegarder avec `CTRL + X`, puis `Y` et `Entrée`.  

#### 3.3 Gérer les permissions  
- Modifier les droits d’accès :  
  ```bash
  chmod +x script.sh  # Rend le script exécutable
  chmod 777 fichier    # Donne tous les droits
  ```  

---  

### 4. Gestion des processus et tâches en arrière-plan  

#### 4.1 Voir les processus en cours  
- Afficher les processus actifs :  
  ```bash
  ps aux
  top
  ```  

#### 4.2 Arrêter un processus  
- Identifier le PID d’un processus et le tuer :  
  ```bash
  kill -9 PID
  ```  

#### 4.3 Exécuter en arrière-plan  
- Lancer une commande en arrière-plan :  
  ```bash
  python3 script.py &
  ```  

---  

### 5. Gestion des utilisateurs et accès root  

#### 5.1 Différence entre utilisateur normal et root  
- Par défaut, Termux tourne sans accès root.  
- Si ton téléphone est rooté, installe `tsu` :  
  ```bash
  pkg install tsu
  ```  

#### 5.2 Passer en root  
- Accéder au root (si disponible) :  
  ```bash
  tsu
  ```  

---  

### 6. Redirections et flux d’entrée/sortie  

#### 6.1 Rediriger la sortie  
- Rediriger un résultat vers un fichier :  
  ```bash
  ls > liste.txt
  ```  

#### 6.2 Utiliser les pipes  
- Chainer les commandes :  
  ```bash
  ls | grep "nom_du_fichier"
  ```  

---  

### 7. Installation et utilisation de Python sur Termux  

#### 7.1 Installer Python  
- Vérifier si Python est installé :  
  ```bash
  python --version
  ```  
- Installer Python :  
  ```bash
  pkg install python
  ```  

#### 7.2 Exécuter un script Python  
- Créer un script simple :  
  ```bash
  nano script.py
  ```  
- Ajouter le code suivant :  
  ```python
  print("Hello, Termux!")
  ```  
- Exécuter le script :  
  ```bash
  python script.py
  ```  

---  

### 8. Automatisation avec des scripts  

#### 8.1 Créer un script Bash  
- Créer un fichier `script.sh` :  
  ```bash
  nano script.sh
  ```  
- Ajouter du contenu :  
  ```bash
  #!/data/data/com.termux/files/usr/bin/bash
  echo "Ce script tourne dans Termux"
  ```  
- Rendre le script exécutable :  
  ```bash
  chmod +x script.sh
  ./script.sh
  ```  

---  

### 9. Accès au réseau et commandes utiles  

#### 9.1 Tester la connexion Internet  
- Vérifier si le réseau fonctionne :  
  ```bash
  ping google.com
  ```  
- Télécharger un fichier avec `wget` :  
  ```bash
  wget http://example.com/fichier.txt
  ```  

#### 9.2 Scanner un réseau local  
- Installer `nmap` et scanner un réseau :  
  ```bash
  pkg install nmap
  nmap -sP 192.168.1.1/24
  ```  

---  

### 10. Personnalisation de Termux  

#### 10.1 Modifier l’invite de commande  
- Modifier `.bashrc` pour changer le prompt :  
  ```bash
  nano ~/.bashrc
  ```  
- Ajouter :  
  ```bash
  export PS1="[\u@\h]$ "
  ```  

#### 10.2 Ajouter des alias  
- Ouvrir `.bashrc` et ajouter des alias :  
  ```bash
  alias ll="ls -lah"
  alias update="pkg update && pkg upgrade"
  ```  

---  

### 11. Sécurité et protection des données  

#### 11.1 Chiffrer des fichiers  
- Installer GPG et chiffrer un fichier :  
  ```bash
  pkg install gnupg
  gpg -c fichier.txt
  ```  

#### 11.2 Sauvegarder et compresser des fichiers  
- Compresser un dossier :  
  ```bash
  tar -cvzf archive.tar.gz mon_dossier
  ```  

---  

### 12. Projets pratiques  

#### 12.1 Automatiser une sauvegarde  
- Script pour copier un dossier automatiquement :  
  ```bash
  rsync -av ~/Documents/ /storage/emulated/0/Backup/
  ```  

#### 12.2 Créer un serveur HTTP  
- Lancer un serveur avec Python :  
  ```bash
  python -m http.server 8080
  ```  

---  
