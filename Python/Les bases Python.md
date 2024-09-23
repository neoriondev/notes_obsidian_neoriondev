### Les saisies utilisateur sont stockées dans une variable :

Une saisie de l'utilisateur peut être récupérée et stockée dans une variable avec la fonction `input()`. Par exemple :
``
``a = input("Quel âge as-tu ?")
``print(a)

- **`a`** stocke la valeur entrée par l'utilisateur.
- La fonction **`input()`** renvoie toujours une chaîne de caractères (texte), même si l'utilisateur entre un nombre.

### Conversion de types :

Parfois, on a besoin de convertir cette chaîne en un autre type (comme un entier ou un nombre à virgule flottante).

- **`int()`** : Convertit une chaîne de caractères en un entier (uniquement pour des valeurs numériques sans virgule).

``age = int(input("Quel âge as-tu ?"))
``print(age)

* `float()` : Convertit une chaîne de caractères en un nombre à virgule flottante (pour des nombres avec virgule).

``poids = float(input("Quel est ton poids ?"))
``print(poids)

### Arrondir les nombres :

- **`round()`** : Permet d'arrondir un nombre à un certain nombre de chiffres après la virgule.

``valeur = 3.14159
``valeur_arrondie = round(valeur, 2)  # Arrondit à 2 chiffres après la virgule
``print(valeur_arrondie)  # Résultat : 3.14

### Styles de nommage des variables :

1. **camelCase** : Le premier mot est en minuscule, et chaque mot suivant commence par une majuscule. Utilisé dans d'autres langages comme JavaScript.
    
    - Exemple : `nombreDeVictoires`
2. **snake_case** (utilisé en Python) : Tous les mots sont en minuscules et séparés par des underscores (_).
    
    - Exemple : `nombre_de_victoires`
3. **lowerCamelCase** : Similaire au camelCase, mais on commence avec une majuscule (souvent utilisé pour nommer des classes).
    
    - Exemple : `NomDeClasse`
4. **UpperCamelCase** : Toutes les premières lettres des mots sont en majuscules.
    
    - Exemple : `NomDeVariable`
5. **kebab-case** : Utilisé dans certains environnements comme les fichiers CSS. Les mots sont en minuscules et séparés par des tirets.
    
    - Exemple : `nombre-de-victoires`
6. **Kebab-Case** : Variante avec les majuscules en début de chaque mot.
    
    - Exemple : `Nombre-De-Victoires`


# Structures de Contrôle :
``if, elif, else`` pour les structures conditionnelles.
``for`` et ``while`` pour les boucles.
Les blocs de code associés sont également délimités par l'indentation.

```python

if condition:
    # Bloc de code si la condition est vraie
    print("Condition vraie")
elif autre_condition:
    # Bloc de code si une autre condition est vraie
    print("Autre condition vraie")
else:
    # Bloc de code si aucune condition n'est vraie
    print("Aucune condition vraie")

for element in iterable:
    # Bloc de code à exécuter pour chaque élément de l'itérable
    print(element)

while condition:
    # Bloc de code à exécuter tant que la condition est vraie
    print("Condition vraie")
    condition = False  # Pour éviter une boucle infinie
    ```

# Opérateur de comparaison

Les opérateur de comparaison répondent toujours pas True ou False

* ``==`` On vérifie si une valeur est strictement égal à une autre valeur

* ``!=`` On vérifie si une valeur est différente à une autre valeur

- ``>`` On vérifie si une valeur est supérieur à une autre valeur

- ``<``  On vérifie si une valeur est inférieur à une autre valeur

- ``<=`` On vérifie si une valeur est inférieur ou égal à une autre valeur

- ``>=`` On vérifie si une valeur est supérieur ou égal à une autre valeur