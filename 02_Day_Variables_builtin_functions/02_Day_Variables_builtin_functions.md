# 30-Days-of-Python-on-Termux 🐍📱

[Revenir au sommaire](../README.md) | [Jour 3 : Entrées/Sorties >>](../03_Day_Input_Output/03_input_output.md)

## 📘 Jour 2 : Syntaxe de base (variables, types de données, opérations, fonctions intégrées)

Bienvenue dans le **Jour 2** de *30 Days of Python on Termux* ! Aujourd'hui, nous allons plonger dans les fondamentaux de Python : les **variables**, les **types de données**, les **opérations** de base, et une exploration approfondie des **fonctions intégrées** (built-in functions). Ce cours est conçu pour vous donner une base solide avec de nombreux exemples pratiques que vous pouvez tester directement dans Termux. À la fin, vous serez à l'aise pour manipuler des données, effectuer des calculs, et utiliser les outils intégrés de Python pour résoudre des problèmes.

---

## 🎯 Objectifs d'apprentissage

- Comprendre et utiliser les **variables** pour stocker et manipuler des données.
- Maîtriser les principaux **types de données** de Python.
- Réaliser des **opérations** arithmétiques, logiques et sur les chaînes.
- Découvrir et appliquer un large éventail de **fonctions intégrées** de Python.
- Pratiquer avec des exercices variés pour renforcer vos compétences.

---

## 1. Les variables : stocker des données

Une **variable** est un conteneur qui stocke une valeur (nombre, texte, liste, etc.). En Python, vous créez une variable en lui attribuant une valeur avec le signe `=`. Aucune déclaration préalable n'est nécessaire, ce qui rend Python simple et flexible.

### Syntaxe
```python
nom_de_variable = valeur
```

### Exemples
```python
age = 18
nom = "Elhadj"
prix = 19.99
est_etudiant = True
fruits = ["pomme", "banane", "orange"]
```

- `age` contient un entier (`int`).
- `nom` contient une chaîne de caractères (`str`).
- `prix` contient un flottant (`float`).
- `est_etudiant` contient un booléen (`bool`).
- `fruits` contient une liste (`list`).

### Tester dans Termux
1. Ouvre le shell Python :
   ```bash
   python
   ```
2. Essaye ces commandes :
   ```python
   >>> age = 18
   >>> print(age)
   30
   >>> nom = "Elhadj"
   >>> print("Bonjour, " + nom)
   Bonjour, Elhadj
   >>> fruits = ["pomme", "banane"]
   >>> print(fruits)
   ['pomme', 'banane']
   ```

### Règles pour nommer les variables
- **Valides** : Lettres (a-z, A-Z), chiffres (0-9), underscores `_`. Exemple : `mon_age`, `nombre2`.
- **Première lettre** : Lettre ou underscore, pas un chiffre. Exemple : `_variable` (valide), `2variable` (invalide).
- **Mots réservés** : Évite les mots clés de Python comme `if`, `for`, `print`. Liste complète : `help("keywords")` dans le shell Python.
- **Conseil** : Utilise des noms descriptifs, par exemple `salaire_mensuel` plutôt que `s`.

**Exemples corrects** :
```python
compteur_de_points = 100
nom_complet = "Elhadj Oumar Rafiou Bah"
_prix_cache = 99.99
```

**Exemples incorrects** :
```python
2score = 100  # Erreur : commence par un chiffre
for = "test"  # Erreur : mot réservé
nom-variable = "Alice"  # Erreur : tiret non autorisé
```

### Exemple pratique
Crée un fichier `variables.py` :
```bash
nano variables.py
```
Ajoute ce code :
```python
# Exemple de variables
prenom = "Elhadj"
age = 18
ville = "Conakry"
est_actif = True
hobbies = ["coder", "lire", "flemmarder", "physique"]

print("Prénom :", prenom)
print("Âge :", age)
print("Ville :", ville)
print("Actif ?", est_actif)
print("Hobbies :", hobbies)
```
Exécute :
```bash
python variables.py
```
**Sortie** :
```
Prénom : Elhadj
Âge : 18
Ville : Conakry
Actif ? True
Hobbies : ['coder', 'lire', 'flemmarder', 'physique']
```

---

## 2. Types de données

Python prend en charge plusieurs types de données pour gérer différents types d'informations. Voici un tableau récapitulatif avec des exemples :

| Type | Description | Exemple |
|------|-------------|---------|
| `int` | Entier | `42`, `-10`, `0` |
| `float` | Nombre décimal | `3.14`, `-0.001`, `2.0` |
| `str` | Chaîne de caractères | `"Bonjour"`, `'Termux'` |
| `bool` | Booléen | `True`, `False` |
| `list` | Liste ordonnée, modifiable | `[1, 2, 3]`, `["pomme", "banane"]` |
| `tuple` | Liste ordonnée, non modifiable | `(1, 2, 3)`, `("a", "b")` |
| `dict` | Dictionnaire (clé-valeur) | `{"nom": "Elhadj Oumar Rafiou", "age": 18}` |
| `set` | Ensemble d'éléments uniques | `{1, 2, 3}`, `{"chat", "chien"}` |

### Vérifier le type
Utilise la fonction `type()` pour connaître le type d'une valeur :
```python
>>> print(type(42))
<class 'int'>
>>> print(type(3.14))
<class 'float'>
>>> print(type("Termux"))
<class 'str'>
>>> print(type([1, 2, 3]))
<class 'list'>
>>> print(type({"nom": "Elhadj Oumar Rafiou"}))
<class 'dict'>
```

### Exemple pratique
Crée un fichier `types_donnees.py` :
```bash
nano types_donnees.py
```
Ajoute :
```python
# Vérification des types de données
entier = 100
flottant = 3.14159
texte = "Python sur Termux"
booleen = False
liste = [1, "deux", 3.0]
tuple = (10, 20)
dictionnaire = {"pays": "Guinée", "capitale": "Conakry"}
ensemble = {1, 2, 3, 3}  # 3 n'apparaît qu'une fois

print("Entier :", type(entier))
print("Flottant :", type(flottant))
print("Texte :", type(texte))
print("Booléen :", type(booleen))
print("Liste :", type(liste))
print("Tuple :", type(tuple))
print("Dictionnaire :", type(dictionnaire))
print("Ensemble :", type(ensemble), ensemble)  # Affiche l'ensemble sans doublons
```
Exécute :
```bash
python types_donnees.py
```
**Sortie** :
```
Entier : <class 'int'>
Flottant : <class 'float'>
Texte : <class 'str'>
Booléen : <class 'bool'>
Liste : <class 'list'>
Tuple : <class 'tuple'>
Dictionnaire : <class 'dict'>
Ensemble : <class 'set'> {1, 2, 3}
```

---

## 3. Opérations de base

Python permet d'effectuer des opérations sur les nombres, les chaînes, et les booléens.

### 3.1 Opérations arithmétiques
| Opérateur | Description | Exemple |
|-----------|-------------|---------|
| `+` | Addition | `10 + 5 = 15` |
| `-` | Soustraction | `10 - 5 = 5` |
| `*` | Multiplication | `10 * 5 = 50` |
| `/` | Division | `10 / 3 = 3.333...` |
| `//` | Division entière | `10 // 3 = 3` |
| `%` | Modulo (reste) | `10 % 3 = 1` |
| `**` | Exponentiation | `2 ** 3 = 8` |

**Exemple dans Termux** :
```python
>>> a = 10
>>> b = 3
>>> print(a + b)   # 13
>>> print(a - b)   # 7
>>> print(a * b)   # 30
>>> print(a / b)   # 3.3333333333333335
>>> print(a // b)  # 3
>>> print(a % b)   # 1
>>> print(a ** 2)  # 100
```

### Exemple pratique
Crée un fichier `operations.py` :
```bash
nano operations.py
```
Ajoute :
```python
# Opérations arithmétiques
x = 15
y = 4

print("Addition :", x + y)       # 19
print("Soustraction :", x - y)   # 11
print("Multiplication :", x * y) # 60
print("Division :", x / y)       # 3.75
print("Division entière :", x // y)  # 3
print("Modulo :", x % y)         # 3
print("Exponentiation :", x ** 2)  # 225
```
Exécute :
```bash
python operations.py
```

### 3.2 Opérations sur les chaînes
- **Concaténation** (`+`) : Combine des chaînes.
- **Répétition** (`*`) : Répète une chaîne.

**Exemple** :
```python
>>> prenom = "Elhadj Oumar Rafiou"
>>> nom = "Bah"
>>> print(prenom + " " + nom)  # Elhadj Bah
>>> print(prenom * 3)          # ElhadjElhadjElhadj
```

**Exemple pratique** :
Crée un fichier `chaines.py` :
```bash
nano chaines.py
```
Ajoute :
```python
# Manipulation de chaînes
titre = "30 Days of Python"
lieu = "Termux"
message = titre + " sur " + lieu
repete = lieu * 3

print("Message :", message)    # 30 Days of Python sur Termux
print("Répétition :", repete)  # TermuxTermuxTermux
print("Longueur :", len(message))  # 20
```
Exécute :
```bash
python chaines.py
```

### 3.3 Opérations booléennes
Les opérateurs booléens permettent de comparer des valeurs ou de combiner des conditions.

| Opérateur | Description | Exemple |
|-----------|-------------|---------|
| `==` | Égal à | `5 == 5` → `True` |
| `!=` | Différent de | `5 != 3` → `True` |
| `<`, `>` | Inférieur, supérieur | `5 < 3` → `False` |
| `<=`, `>=` | Inférieur ou égal, supérieur ou égal | `5 <= 5` → `True` |
| `and` | Et logique | `True and False` → `False` |
| `or` | Ou logique | `True or False` → `True` |
| `not` | Négation | `not True` → `False` |

**Exemple** :
```python
>>> x = 10
>>> y = 5
>>> print(x > y)        # True
>>> print(x == y * 2)   # True
>>> print(x < y)        # False
>>> print(x >= 10)      # True
>>> print(True and False)  # False
>>> print(True or False)   # True
>>> print(not True)        # False
```

**Exemple pratique** :
Crée un fichier `booleens.py` :
```bash
nano booleens.py
```
Ajoute :
```python
# Opérations booléennes
age = 18
est_majeur = age >= 18
est_etudiant = True

print("Âge :", age)
print("Majeur ?", est_majeur)          # True
print("Étudiant et majeur ?", est_majeur and est_etudiant)  # True
print("Étudiant ou majeur ?", est_majeur or est_etudiant)   # True
print("Non étudiant ?", not est_etudiant)  # False
```
Exécute :
```bash
python booleens.py
```

---

## 4. Fonctions intégrées (Built-in Functions)

Python propose plus de **60 fonctions intégrées** pour simplifier la programmation. Voici une liste élargie des fonctions les plus utiles pour les débutants, avec des exemples pratiques.

| Fonction | Description | Exemple |
|----------|-------------|---------|
| `print()` | Affiche une valeur | `print("Hello")` |
| `type()` | Retourne le type d'une valeur | `type(42)` → `<class 'int'>` |
| `len()` | Retourne la longueur (chaîne, liste, etc.) | `len("Python")` → `6` |
| `int()` | Convertit en entier | `int("10")` → `10` |
| `float()` | Convertit en flottant | `float("3.14")` → `3.14` |
| `str()` | Convertit en chaîne | `str(42)` → `"42"` |
| `input()` | Demande une entrée utilisateur | `nom = input("Votre nom : ")` |
| `abs()` | Valeur absolue | `abs(-5)` → `5` |
| `round()` | Arrondit un nombre | `round(3.14159, 2)` → `3.14` |
| `min()` | Retourne le minimum | `min(1, 2, 3)` → `1` |
| `max()` | Retourne le maximum | `max(1, 2, 3)` → `3` |
| `sum()` | Somme d'une liste | `sum([1, 2, 3])` → `6` |
| `pow()` | Calcule une puissance | `pow(2, 3)` → `8` |
| `sorted()` | Trie une liste | `sorted([3, 1, 2])` → `[1, 2, 3]` |
| `chr()` | Convertit un code ASCII en caractère | `chr(65)` → `'A'` |
| `ord()` | Convertit un caractère en code ASCII | `ord('A')` → `65` |

### Exemples pratiques
1. **Utilisation de `input()` et `len()`** :
   ```python
   >>> nom = input("Entrez votre nom : ")
   Entrez votre nom : Elhadj
   >>> print("Longueur du nom :", len(nom))
   Longueur du nom : 6
   ```

2. **Utilisation de `abs()` et `round()`** :
   ```python
   >>> nombre = -7.56789
   >>> print("Valeur absolue :", abs(nombre))
   Valeur absolue : 7.56789
   >>> print("Arrondi à 2 décimales :", round(nombre, 2))
   Arrondi à 2 décimales : -7.57
   ```

3. **Utilisation de `min()`, `max()`, `sum()`** :
   ```python
   >>> nombres = [10, 5, 8, 12, 3]
   >>> print("Minimum :", min(nombres))
   Minimum : 3
   >>> print("Maximum :", max(nombres))
   Maximum : 12
   >>> print("Somme :", sum(nombres))
   Somme : 38
   ```

4. **Utilisation de `sorted()`** :
   ```python
   >>> fruits = ["banane", "pomme", "orange"]
   >>> print("Trié :", sorted(fruits))
   Trié : ['banane', 'orange', 'pomme']
   ```

5. **Utilisation de `chr()` et `ord()`** :
   ```python
   >>> print(chr(97))  # Convertit le code ASCII 97 en caractère
   a
   >>> print(ord('b'))  # Convertit le caractère 'b' en code ASCII
   98
   ```

**Script combiné** :
Crée un fichier `builtins.py` :
```bash
nano builtins.py
```
Ajoute :
```python
# Exemple de fonctions intégrées
nombres = [7, 2, 9, 4, 1]
texte = "Python sur Termux"
nombre = -15.6789

print("Liste originale :", nombres)
print("Minimum :", min(nombres))
print("Maximum :", max(nombres))
print("Somme :", sum(nombres))
print("Liste triée :", sorted(nombres))
print("Longueur du texte :", len(texte))
print("Valeur absolue :", abs(nombre))
print("Arrondi :", round(nombre, 1))
print("Caractère ASCII 65 :", chr(65))
print("Code ASCII de 'A' :", ord('A'))
```
Exécute :
```bash
python builtins.py
```
**Sortie** :
```
Liste originale : [7, 2, 9, 4, 1]
Minimum : 1
Maximum : 9
Somme : 23
Liste triée : [1, 2, 4, 7, 9]
Longueur du texte : 17
Valeur absolue : 15.6789
Arrondi : -15.7
Caractère ASCII 65 : A
Code ASCII de 'A' : 65
```

---

## 5. Conversion de types (Type Casting)

Vous pouvez convertir un type de données en un autre avec des fonctions comme `int()`, `float()`, `str()`, etc.

### Exemples
```python
>>> nombre = "42"
>>> print(int(nombre) + 8)  # Convertit en entier
50
>>> print(float(nombre))    # Convertit en flottant
42.0
>>> print(str(42) + " ans")  # Convertit en chaîne
42 ans
>>> print(list("Python"))    # Convertit une chaîne en liste
['P', 'y', 't', 'h', 'o', 'n']
```

### Attention aux erreurs
```python
>>> int("abc")  # Erreur : impossible de convertir "abc" en entier
ValueError: invalid literal for int() with base 10: 'abc'
```

**Exemple pratique** :
Crée un fichier `conversion.py` :
```bash
nano conversion.py
```
Ajoute :
```python
# Conversion de types
age_texte = "25"
prix_texte = "19.99"
mot = "Termux"

age = int(age_texte)
prix = float(prix_texte)
lettres = list(mot)

print("Âge + 5 :", age + 5)              # 30
print("Prix avec TVA (20%) :", prix * 1.2)  # 23.988
print("Lettres du mot :", lettres)        # ['T', 'e', 'r', 'm', 'u', 'x']
```
Exécute :
```bash
python conversion.py
```

---

## 6. Script pratique complet

Créons un script qui combine variables, opérations, fonctions intégrées, et entrées utilisateur.

1. Crée un fichier `jour2_projet.py` :
   ```bash
   nano jour2_projet.py
   ```
2. Ajoute ce code :
   ```python
   # Jour 2 - Défi 30DaysOfPython
   prenom = input("Entrez votre prénom : ")
   age = int(input("Entrez votre âge : "))
   nombres = [10, 20, 30, 40, 50]

   # Calculs
   annee_naissance = 2025 - age
   message = "Bonjour, " + prenom + " ! Vous êtes né(e) vers " + str(annee_naissance) + "."
   somme_nombres = sum(nombres)
   min_nombres = min(nombres)
   max_nombres = max(nombres)
   nombres_tries = sorted(nombres)

   # Affichage
   print(message)
   print("Longueur du message :", len(message))
   print("Type de l'âge :", type(age))
   print("Type du prénom :", type(prenom))
   print("Somme des nombres :", somme_nombres)
   print("Nombre minimum :", min_nombres)
   print("Nombre maximum :", max_nombres)
   print("Nombres triés :", nombres_tries)
   ```
3. Exécute :
   ```bash
   python jour2_projet.py
   ```
   **Sortie** (exemple) :
   ```
   Entrez votre prénom : Elhadj
   Entrez votre âge : 25
   Bonjour, Elhadj ! Vous êtes né(e) vers 2000.
   Longueur du message : 39
   Type de l'âge : <class 'int'>
   Type du prénom : <class 'str'>
   Somme des nombres : 150
   Nombre minimum : 10
   Nombre maximum : 50
   Nombres triés : [10, 20, 30, 40, 50]
   ```

---

## 7. Exercices pour pratiquer

1. **Variables et opérations** :
   - Crée des variables `x = 20` et `y = 7`.
   - Affiche les résultats de `x + y`, `x - y`, `x * y`, `x / y`, `x // y`, `x % y`, `x ** 2`.
   - Exemple :
     ```python
     x = 20
     y = 7
     print("Addition :", x + y)
     ```

2. **Entrée utilisateur** :
   - Écris un script qui demande deux nombres à l'utilisateur, les convertit en entiers, et affiche leur somme, produit, division, et modulo.

3. **Manipulation de chaînes** :
   - Crée une variable avec ton nom complet.
   - Affiche ton nom en majuscules (`upper()`), en minuscules (`lower()`), et sa longueur (`len()`).
   - Exemple :
     ```python
     nom = "Elhadj Bah"
     print(nom.upper())
     ```

4. **Conversion de types** :
   - Demande à l'utilisateur un prix sous forme de chaîne (ex. : `"29.99"`).
   - Convertis-le en flottant et ajoute une taxe de 15 %.
   - Affiche le résultat avec deux décimales (`round()`).

5. **Fonctions intégrées** :
   - Crée une liste `scores = [85, 92, 78, 95, 88]`.
   - Affiche le minimum, le maximum, la somme, et la liste triée avec `min()`, `max()`, `sum()`, et `sorted()`.

6. **Défi** :
   - Écris un script qui :
     - Demande le prénom, l'âge, et la ville de l'utilisateur.
     - Calcule l'année de naissance (année actuelle = 2025).
     - Affiche un message comme : `"Salut [prenom], tu as [âge] ans, né(e) vers [année] à [ville]."`
     - Affiche la longueur du message et les types des variables utilisées.

---

## 💡 Conseils pour réussir

- **Teste dans le shell** : Ouvre `python` et essaie chaque concept avant de l'écrire dans un fichier.
- **Débogue** : Lis attentivement les messages d'erreur (`SyntaxError`, `TypeError`, etc.) pour corriger ton code.
- **Expérimente** : Modifie les exemples pour voir comment ils réagissent.
- **Pratique quotidienne** : Consacre 30 à 60 minutes par jour pour assimiler les concepts.
- **Rejoins la communauté** : Pose tes questions via les [issues GitHub](https://github.com/EORBAH/30-Days-of-Python-on-Termux/issues).

---

## 📢 Appel à l’action

Félicitations, tu as maîtrisé les bases de la syntaxe Python et les fonctions intégrées ! Continue à pratiquer avec les exercices et passe au **Jour 3** pour explorer les entrées/sorties (`input/output`).

[Revenir au sommaire](../README.md) | [Jour 3 : Entrées/Sorties >>](../03_Day_Input_Output/03_input_output.md)

---

## 🤝 Contribuer

Tu veux améliorer cette leçon ? Contribue au projet :
1. Fork le dépôt [30-Days-of-Python-on-Termux](https://github.com/EORBAH/30-Days-of-Python-on-Termux).
2. Crée une branche : `git checkout -b jour2-amelioration`.
3. Commite tes changements : `git commit -m "Amélioration Jour 2"`.
4. Pousse : `git push origin jour2-amelioration`.
5. Ouvre une Pull Request.

---

## 🌐 Autres langues

- [English](../Course/en/README.md)
- [中文](../Course/cn/README.md)

---

⭐ **Aime ce projet ? Donne-lui une étoile sur GitHub !**

Suivez-nous pour plus d’astuces :  
[![Suivez-nous sur X](https://img.shields.io/badge/X-Follow-black?logo=x)](https://x.com/eor_bah545)  
[![Suivez-nous sur Telegram](https://img.shields.io/badge/Telegram-Follow-black?logo=telegram)](https://t.me/phoenix_for_developers)  
[![Suivez-nous sur YouTube](https://img.shields.io/badge/YouTube-Follow-black?logo=youtube)](https://youtube.com/@eor_bah545)
