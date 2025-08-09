# 30-Days-of-Python-on-Termux 🐍📱

Bienvenue dans **30-Days-of-Python-on-Termux**, un cours intensif de 30 jours pour apprendre à coder en Python directement depuis votre smartphone Android avec **Termux** ! Que vous soyez débutant ou que vous souhaitiez approfondir vos compétences, ce programme vous guide des bases aux projets avancés, transformant votre téléphone en une station de codage portable.

---

## 📘 Pourquoi ce cours ?

- **Codez n'importe où** : Apprenez Python sur votre téléphone, dans les transports, en voyage ou chez vous.
- **Progression claire** : 30 jours structurés, du niveau débutant à avancé, avec des leçons, exemples de code et exercices pratiques.
- **Projets concrets** : Créez des applications comme une calculatrice, un gestionnaire de tâches ou un analyseur de logs.
- **Gratuit et open-source** : Accédez à tout le contenu et contribuez via [GitHub](https://github.com/EORBAH/30-Days-of-Python-on-Termux).

---

## 🚀 Comment démarrer ?

1. **Installez Termux** :
   - Téléchargez Termux depuis [F-Droid](https://f-droid.org/packages/com.termux/) (évitez le Play Store, la version n’est plus à jour).
   - Mettez à jour Termux :
     ```bash
     pkg update && pkg upgrade
     ```
   - Installez Python :
     ```bash
     pkg install python
     ```

2. **Clonez le dépôt** :
   ```bash
   git clone https://github.com/EORBAH/30-Days-of-Python-on-Termux.git
   cd 30-Days-of-Python-on-Termux
   ```

3. **Commencez le cours** : Suivez les leçons quotidiennement, testez les exemples et réalisez les exercices.

---

## 📚 Structure du cours

Le cours est organisé en **5 modules** sur 30 jours, plus un **module bonus** pour des projets professionnels. Chaque jour inclut une leçon théorique, des exemples de code et des exercices pratiques.

### Module 1 : Les bases de Python (Jours 1-7)
Maîtrisez les fondamentaux de Python pour une base solide.

| Jour | Cours |
|------|---------------------------------------------------------|
| 1    | [Introduction à Python et Termux](./01_Day_Introduction/01_introduction.md) |
| 2    | [Syntaxe de base (variables, types de données, opérations)](./02_Day_Variables_builtin_functions/02_variables_builtin_functions.md) |
| 3    | [Entrées/sorties (input/output, print)](./03_Day_Input_Output/03_input_output.md) |
| 4    | [Structures conditionnelles (if, else, elif)](./04_Day_Conditionals/04_conditionals.md) |
| 5    | [Boucles (for, while)](./05_Day_Loops/05_loops.md) |
| 6    | [Listes, tuples et ensembles](./06_Day_Lists_Tuples_Sets/06_lists_tuples_sets.md) |
| 7    | [Projet : Mini-calculatrice](./07_Day_Mini_Project_Calculator/07_mini_calculator.md) |

### Module 2 : Structures de données et fonctions (Jours 8-14)
Approfondissez les structures de données et les fonctions.

| Jour | Cours |
|------|---------------------------------------------------------|
| 8    | [Dictionnaires et manipulation de données](./08_Day_Dictionaries/08_dictionaries.md) |
| 9    | [Fonctions et portée des variables](./09_Day_Functions/09_functions.md) |
| 10   | [Arguments de fonctions (par défaut, *args, **kwargs)](./10_Day_Function_Arguments/10_function_arguments.md) |
| 11   | [Gestion des erreurs (try, except)](./11_Day_Error_Handling/11_error_handling.md) |
| 12   | [Manipulation de chaînes de caractères](./12_Day_Strings/12_strings.md) |
| 13   | [Introduction aux modules et pip](./13_Day_Modules_Pip/13_modules_pip.md) |
| 14   | [Projet : Gestionnaire de tâches simple](./14_Day_Mini_Project_Task_Manager/14_task_manager.md) |

### Module 3 : Programmation orientée objet (Jours 15-21)
Structurez votre code avec la programmation orientée objet.

| Jour | Cours |
|------|---------------------------------------------------------|
| 15   | [Classes et objets](./15_Day_Classes_Objects/15_classes_objects.md) |
| 16   | [Méthodes et attributs](./16_Day_Methods_Attributes/16_methods_attributes.md) |
| 17   | [Héritage et polymorphisme](./17_Day_Inheritance_Polymorphism/17_inheritance_polymorphism.md) |
| 18   | [Encapsulation et propriétés](./18_Day_Encapsulation_Properties/18_encapsulation_properties.md) |
| 19   | [Modules avancés (datetime, random)](./19_Day_Advanced_Modules/19_advanced_modules.md) |
| 20   | [Introduction aux bibliothèques externes](./20_Day_External_Libraries/20_external_libraries.md) |
| 21   | [Projet : Jeu de devinettes orienté objet](./21_Day_Mini_Project_Guessing_Game/21_guessing_game.md) |

### Module 4 : Manipulation de fichiers et automatisation (Jours 22-26)
Automatisez des tâches et manipulez des fichiers.

| Jour | Cours |
|------|---------------------------------------------------------|
| 22   | [Lecture et écriture de fichiers](./22_Day_File_Handling/22_file_handling.md) |
| 23   | [Gestion des fichiers CSV](./23_Day_CSV_Handling/23_csv_handling.md) |
| 24   | [Automatisation avec os et shutil](./24_Day_Automation/24_automation_os_shutil.md) |
| 25   | [Introduction aux expressions régulières](./25_Day_Regular_Expressions/25_regular_expressions.md) |
| 26   | [Projet : Analyseur de logs simple](./26_Day_Mini_Project_Log_Analyzer/26_log_analyzer.md) |

### Module 5 : Projets avancés et révision (Jours 27-30)
Consolidez vos compétences avec des projets avancés.

| Jour | Cours |
|------|---------------------------------------------------------|
| 27   | [Introduction à l’API REST avec requests](./27_Day_REST_API/27_rest_api.md) |
| 28   | [Scripting avancé avec Termux](./28_Day_Advanced_Scripting/28_advanced_scripting.md) |
| 29   | [Optimisation et bonnes pratiques](./29_Day_Best_Practices/29_best_practices.md) |
| 30   | [Projet final : Application d’automatisation personnalisée](./30_Day_Final_Project/30_final_project.md) |

### Module Bonus : Projets professionnels
Explorez des sujets avancés pour des applications professionnelles.

| Jour | Cours |
|------|---------------------------------------------------------|
| +1   | [Web Scraping](./Bonus_Day_1_Web_Scraping/bonus_web_scraping.md) |
| +2   | [Statistiques avec NumPy](./Bonus_Day_2_Numpy/bonus_numpy.md) |
| +3   | [Développement web avec Python](./Bonus_Day_3_Web_Dev/bonus_web_dev.md) |
| +4   | [Python avec MongoDB](./Bonus_Day_4_MongoDB/bonus_mongodb.md) |
| +5   | [Conception d'API](./Bonus_Day_5_API_Design/bonus_api_design.md) |
| +6   | [Analyse de données avec Pandas](./Bonus_Day_6_Pandas/bonus_pandas.md) |
| +7   | [Data Engineering](./Bonus_Day_7_Data_Engineering/bonus_data_engineering.md) |

---
EN [English](./Course/en/README.md)
CN [中文](./Course/cn/README.md)

[Day 2 >>](./02_Day_Variables_builtin_functions/02_variables_builtin_functions.md)

[![Suivez-nous sur X](https://img.shields.io/badge/X-Follow-black?logo=x)](https://x.com/eor_bah545)  [![Suivez-nous sur telegram](https://img.shields.io/badge/telegram-Follow-black?logo=telegram)](https://t.me/phoenix_for_developers)  [![Suivez-nous sur youtube](https://img.shields.io/badge/youtube-Follow-black?logo=youtube)](https://youtube.com/@eor_bah545)

# 📘 Jour 1


## 💻 Les bases de Termux de A à Z

Pour bien démarrer, voici un guide essentiel pour maîtriser **Termux**, l'environnement idéal pour coder en Python sur Android.

### 1. Introduction à Termux

#### 1.1 Qu'est-ce que Termux ?
Termux est un émulateur de terminal pour Android offrant un environnement Linux complet. Il permet d'exécuter des commandes Unix/Linux, d'écrire des scripts et de coder en Python ou autres langages.

#### 1.2 Installation de Termux
- Téléchargez Termux depuis [F-Droid](https://f-droid.org/packages/com.termux/) ou le [site officiel](https://termux.dev).
- **Important** : Évitez la version du Play Store, qui n’est plus maintenue.

#### 1.3 Premiers pas
Ouvrez Termux et testez :
```bash
echo "Bienvenue dans Termux !"
```
Commandes essentielles :
```bash
pwd        # Affiche le répertoire actuel
ls         # Liste les fichiers et dossiers
cd         # Change de dossier
mkdir      # Crée un dossier
rm         # Supprime un fichier
```

---

### 2. Gestion des paquets et mises à jour

#### 2.1 Mettre à jour Termux
Avant tout, mettez à jour :
```bash
pkg update && pkg upgrade
```

#### 2.2 Installer et supprimer des paquets
- Installer Python :
  ```bash
  pkg install python
  ```
- Désinstaller un paquet :
  ```bash
  pkg uninstall python
  ```

#### 2.3 Rechercher des paquets
- Lister les paquets disponibles :
  ```bash
  pkg list-all
  ```
- Rechercher un paquet :
  ```bash
  pkg search nano
  ```

---

### 3. Gestion des fichiers et permissions

#### 3.1 Commandes de base
- Créer un fichier ou dossier :
  ```bash
  touch fichier.txt
  mkdir mon_dossier
  ```
- Copier ou déplacer :
  ```bash
  cp fichier.txt mon_dossier/
  mv fichier.txt mon_dossier/
  ```
- Supprimer :
  ```bash
  rm fichier.txt
  rm -rf mon_dossier
  ```

#### 3.2 Modifier un fichier
- Installer `nano` :
  ```bash
  pkg install nano
  nano fichier.txt
  ```
- Sauvegardez avec `CTRL + X`, `Y`, `Entrée`.

#### 3.3 Gérer les permissions
- Rendre un script exécutable :
  ```bash
  chmod +x script.sh
  ```
- Donner tous les droits :
  ```bash
  chmod 777 fichier
  ```

---

### 4. Gestion des processus et tâches en arrière-plan

#### 4.1 Voir les processus
- Afficher les processus actifs :
  ```bash
  ps aux
  top
  ```

#### 4.2 Arrêter un processus
- Tuer un processus par son PID :
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

#### 5.1 Utilisateur normal vs root
Termux fonctionne par défaut sans accès root. Pour un accès root (si votre téléphone est rooté) :
```bash
pkg install tsu
tsu
```

---

### 6. Redirections et flux d’entrée/sortie

#### 6.1 Rediriger la sortie
- Rediriger vers un fichier :
  ```bash
  ls > liste.txt
  ```

#### 6.2 Utiliser les pipes
- Chainer des commandes :
  ```bash
  ls | grep "nom_du_fichier"
  ```

---

### 7. Installation et utilisation de Python sur Termux

#### 7.1 Installer Python
- Vérifier la version :
  ```bash
  python --version
  ```
- Installer Python :
  ```bash
  pkg install python
  ```

#### 7.2 Exécuter un script Python
- Créer un script :
  ```bash
  nano script.py
  ```
- Ajouter :
  ```python
  print("Hello, Termux!")
  ```
- Exécuter :
  ```bash
  python script.py
  ```

---

### 8. Automatisation avec des scripts

#### 8.1 Créer un script Bash
- Créer un script :
  ```bash
  nano script.sh
  ```
- Ajouter :
  ```bash
  #!/data/data/com.termux/files/usr/bin/bash
  echo "Ce script tourne dans Termux"
  ```
- Rendre exécutable et lancer :
  ```bash
  chmod +x script.sh
  ./script.sh
  ```

---

### 9. Accès au réseau et commandes utiles

#### 9.1 Tester la connexion
- Vérifier le réseau :
  ```bash
  ping google.com
  ```
- Télécharger un fichier :
  ```bash
  wget http://example.com/fichier.txt
  ```

#### 9.2 Scanner un réseau local
- Installer `nmap` et scanner :
  ```bash
  pkg install nmap
  nmap -sP 192.168.1.1/24
  ```

---

### 10. Personnalisation de Termux

#### 10.1 Modifier l’invite de commande
- Éditer `.bashrc` :
  ```bash
  nano ~/.bashrc
  ```
- Ajouter :
  ```bash
  export PS1="[\u@\h]$ "
  ```

#### 10.2 Ajouter des alias
- Ajouter dans `.bashrc` :
  ```bash
  alias ll="ls -lah"
  alias update="pkg update && pkg upgrade"
  ```

---

### 11. Sécurité et protection des données

#### 11.1 Chiffrer des fichiers
- Installer GPG et chiffrer :
  ```bash
  pkg install gnupg
  gpg -c fichier.txt
  ```

#### 11.2 Sauvegarder et compresser
- Compresser un dossier :
  ```bash
  tar -cvzf archive.tar.gz mon_dossier
  ```

---

### 12. Projets pratiques

#### 12.1 Automatiser une sauvegarde
- Script de sauvegarde :
  ```bash
  rsync -av ~/Documents/ /storage/emulated/0/Backup/
  ```

#### 12.2 Créer un serveur HTTP
- Lancer un serveur :
  ```bash
  python -m http.server 8080
  ```

---

## Introduction à Python

### Pourquoi Python ?
Python est un langage de programmation **simple et lisible**, proche du langage humain, ce qui le rend facile à apprendre et à utiliser, même pour les débutants. Sa syntaxe claire permet de se concentrer sur la logique plutôt que sur des détails complexes. Python est largement adopté par des entreprises comme Google, Netflix et Spotify, et il est utilisé dans de nombreux domaines :
- **Développement web** : Créer des sites avec Django ou Flask.
- **Automatisation** : Simplifier des tâches répétitives, comme gérer des fichiers ou envoyer des e-mails.
- **Data Science et IA** : Analyser des données avec Pandas, NumPy, ou construire des modèles d'intelligence artificielle avec TensorFlow.
- **Administration système** : Écrire des scripts pour gérer des serveurs.
- **Applications diverses** : Développer des jeux, des applications de bureau, et bien plus.

Python est un langage incontournable dans le monde de la programmation, et l'apprendre sur **Termux** vous permet de coder directement depuis votre smartphone Android, sans ordinateur, où que vous soyez !

### Configuration de l'environnement sur Termux

#### Installer Python sur Termux
Pour exécuter des scripts Python, vous devez installer Python sur Termux. Suivez ces étapes :
1. Ouvrez Termux (téléchargé depuis [F-Droid](https://f-droid.org/packages/com.termux/), évitez le Play Store).
2. Mettez à jour les paquets :
   ```bash
   pkg update && pkg upgrade
   ```
3. Installez Python :
   ```bash
   pkg install python
   ```
4. Vérifiez que Python est installé :
   ```bash
   python --version
   ```
   **Sortie attendue** (exemple) : `Python 3.11.4` (la version peut varier, mais elle doit être 3.6 ou supérieure).

Si vous voyez la version de Python, félicitations ! Python est prêt à être utilisé sur Termux.

### Le shell interactif de Python
Python est un langage **interprété**, ce qui signifie qu'il exécute le code ligne par ligne sans avoir besoin de compilation. Termux vous permet d'utiliser le **shell interactif de Python** pour tester des commandes immédiatement.

1. Dans Termux, ouvrez le shell Python :
   ```bash
   python
   ```
   Vous verrez l'invite `>>>`, indiquant que Python attend vos commandes.

2. Essayez ce premier script :
   ```python
   >>> print("Hello, World!")
   Hello, World!
   ```
   La fonction `print()` affiche du texte dans le terminal.

3. Testez quelques opérations mathématiques :
   ```python
   >>> 2 + 3
   5
   >>> 3 * 2
   6
   >>> 3 / 2
   1.5
   ```

4. Pour quitter le shell :
   ```python
   >>> exit()
   ```

Si vous faites une erreur, Python affiche un message clair. Par exemple :
```python
>>> print(2 x 3)  # Erreur : 'x' n'est pas un opérateur
SyntaxError: invalid syntax
```
Corrigez en utilisant l'opérateur `*` :
```python
>>> print(2 * 3)
6
```

Le processus de correction des erreurs s'appelle le **débogage**. Vous rencontrerez des erreurs comme `SyntaxError`, `NameError`, `TypeError`, etc. Ces messages vous aident à identifier et corriger les problèmes.

### Premier script Python sur Termux
Le shell interactif est idéal pour tester, mais pour des projets plus complexes, vous écrirez des scripts dans des fichiers `.py`. Voici comment créer votre premier script sur Termux :

1. Créez un fichier `helloworld.py` :
   ```bash
   nano helloworld.py
   ```
2. Ajoutez ce code :
   ```python
   # Jour 1 - Défi 30DaysOfPython
   print("Hello, World!")  # Affiche un message
   print(2 + 3)  # Addition
   print(3 - 1)  # Soustraction
   print(2 * 3)  # Multiplication
   print(3 / 2)  # Division
   print(3 ** 2)  # Exponentielle
   print(3 % 2)  # Modulo
   print(3 // 2)  # Division entière
   ```
3. Sauvegardez (`CTRL + X`, `Y`, `Entrée`) et exécutez :
   ```bash
   python helloworld.py
   ```
   **Sortie** :
   ```
   Hello, World!
   5
   2
   6
   1.5
   9
   1
   1
   ```

### Syntaxe et indentation
Python utilise l'**indentation** (espaces ou tabulations, généralement 4 espaces) pour délimiter les blocs de code, contrairement à d'autres langages qui utilisent des accolades `{}`. Une indentation incorrecte provoque une erreur.

**Exemple correct** :
```python
if 5 > 3:
    print("5 est plus grand que 3")  # Indenté avec 4 espaces
```

**Exemple incorrect** :
```python
if 5 > 3:
print("Erreur !")  # Pas d'indentation
```
**Sortie** : `IndentationError: expected an indented block`

### Commentaires
Les commentaires rendent le code plus lisible. En Python :
- **Commentaire sur une ligne** : Utilisez `#`.
  ```python
  # Ceci est un commentaire
  print("Ce code s'exécute")
  ```
- **Commentaire sur plusieurs lignes** : Utilisez des triples guillemets `"""`.
  ```python
  """Ceci est un commentaire
  sur plusieurs lignes.
  Python l'ignore."""
  ```

### Types de données
Python prend en charge plusieurs types de données. Voici les principaux :
- **Nombres** :
  - **Entiers (int)** : Nombres entiers, ex. : `-3`, `0`, `42`.
  - **Flottants (float)** : Nombres décimaux, ex. : `3.14`, `-0.5`.
  - **Complexes (complex)** : Nombres complexes, ex. : `1 + 2j`.
- **Chaînes de caractères (str)** : Texte entre guillemets simples `'` ou doubles `"`, ex. : `"Bonjour"`, `'Termux'`.
- **Booléens (bool)** : `True` ou `False` (en majuscules).
- **Listes (list)** : Collection ordonnée et modifiable, ex. : `[1, 2, 3]`, `["pomme", "banane"]`.
- **Dictionnaires (dict)** : Collection de paires clé-valeur, ex. : `{"nom": "Alice", "âge": 25}`.
- **Tuples (tuple)** : Collection ordonnée et non modifiable, ex. : `(1, 2, 3)`.
- **Ensembles (set)** : Collection non ordonnée d'éléments uniques, ex. : `{1, 2, 3}`.

**Vérifier les types dans le shell** :
```python
>>> type(10)
<class 'int'>
>>> type(3.14)
<class 'float'>
>>> type("Termux")
<class 'str'>
>>> type([1, 2, 3])
<class 'list'>
```

### Exemple de script avec types de données
Créez un fichier `types_donnees.py` :
```bash
nano types_donnees.py
```
Ajoutez :
```python
# Vérification des types de données
print(type(10))          # Entier
print(type(3.14))        # Flottant
print(type(1 + 3j))      # Complexe
print(type("Eor_bah545"))    # Chaîne
print(type([1, 2, 3]))   # Liste
print(type({"nom": "Elhadj oumar rafiou bah"}))  # Dictionnaire
print(type({9.8, 3.14}))      # Ensemble
print(type((9.8, 3.14)))      # Tuple
```
Exécutez :
```bash
python types_donnees.py
```
**Sortie** :
```
<class 'int'>
<class 'float'>
<class 'complex'>
<class 'str'>
<class 'list'>
<class 'dict'>
<class 'set'>
<class 'tuple'>
```

### Utiliser un éditeur de code sur Termux
Le shell interactif est utile pour tester, mais pour des projets plus complexes, utilisez un éditeur comme `nano` dans Termux. Vous pouvez aussi installer un éditeur plus avancé comme `vim` ou utiliser une application Android compatible avec Termux (ex. : AIDE ou Termux:API pour une expérience plus visuelle).

**Exemple avec nano** :
1. Créez un fichier :
   ```bash
   nano mon_script.py
   ```
2. Écrivez votre code, sauvegardez et exécutez :
   ```bash
   python mon_script.py
   ```

### Conseils pour débuter sur Termux
- **Testez dans le shell** : Expérimentez avec des commandes simples pour comprendre Python.
- **Créez des fichiers .py** : Utilisez `nano` pour écrire des scripts structurés.
- **Déboguez** : Lisez les messages d'erreur pour corriger votre code.
- **Explorez** : Modifiez les exemples pour voir ce qui se passe.

### Exercices pour pratiquer
1. Vérifiez votre version de Python :
   ```bash
   python --version
   ```
2. Dans le shell Python, effectuez ces opérations avec les nombres 3 et 4 :
   ```python
   >>> 3 + 4   # Addition
   >>> 3 - 4   # Soustraction
   >>> 3 * 4   # Multiplication
   >>> 3 / 4   # Division
   >>> 3 ** 4  # Exponentielle
   >>> 3 % 4   # Modulo
   >>> 3 // 4  # Division entière
   ```
3. Écrivez ces chaînes dans le shell :
   ```python
   >>> print("Elhadj oumar rafiou")
   >>> print("Bah")
   >>> print("Guinea")
   >>> print("J'aime les 30 jours de Python")
   ```
4. Vérifiez les types de ces données :
   ```python
   >>> type(10)
   >>> type(9.8)
   >>> type(3.14)
   >>> type(4 - 4j)
   >>> type(['Termux', 'Python', 'Guinea'])
   >>> type("Eor_bah545") 
   ```


## 💡 Conseils pour réussir

- **Pratique quotidienne** : Consacrez 30 à 60 minutes par jour.
- **Expérimentez** : Modifiez les exemples pour mieux comprendre.
- **Rejoignez la communauté** : Posez vos questions via les [issues GitHub](https://github.com/EORBAH/30-Days-of-Python-on-Termux/issues).
- **Amusez-vous** : Profitez de la puissance de Python sur Termux !

---

## 🤝 Contribuer

Ce projet est open-source ! Vous pouvez :
- Proposer des améliorations pour les leçons.
- Ajouter des exercices ou projets.
- Corriger des erreurs.

**Pour contribuer** :
1. Forkez le dépôt.
2. Créez une branche : `git checkout -b feature/nouvelle-fonctionnalite`.
3. Commitez : `git commit -m "Ajout de..."`.
4. Poussez : `git push origin feature/nouvelle-fonctionnalite`.
5. Ouvrez une Pull Request.

---

## 📢 Appel à l’action

Prêt à coder en Python depuis votre poche ? Installez Termux, clonez ce dépôt et lancez-vous dans cette aventure de 30 jours ! Suivez-nous pour des astuces et mises à jour :

[![Suivez-nous sur X](https://img.shields.io/badge/X-Follow-black?logo=x)](https://x.com/eor_bah545)  
[![Suivez-nous sur Telegram](https://img.shields.io/badge/Telegram-Follow-black?logo=telegram)](https://t.me/phoenix_for_developers)  
[![Suivez-nous sur YouTube](https://img.shields.io/badge/YouTube-Follow-black?logo=youtube)](https://youtube.com/@eor_bah545)

⭐ **Aimez ce projet ? Donnez-lui une étoile sur GitHub !**

---

## 🌐 Autres langues

- [English](./Course/en/README.md)
- [中文](./Course/cn/README.md)

---

## 🚀 Passez au Jour 2 !

[Commencer le Jour 2 : Syntaxe de base (variables, types de données, opérations)](./02_Day_Variables_builtin_functions/02_variables_builtin_functions.md)
