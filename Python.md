Debut de doc en PYTHON

Sites de référence : 
- 

# environnement virtuel Venv
- @debian ` apt-get install python3-venv ` installer venv
- @debian `python3 -m venv env & source env/bin/activate ` pour  instancier et activer l'environnement.

# Modules :

# Les paquets :
C'est l'organisation du répertoire et la présence de `__init__.py `  en tête de répertoire qui permettra à python d'interpréter qu'il s'agit d'un paquet
` from mypaquet.lib.mymodule import myclass ` est l'importation qui correspond au répertoire : 
```
  [ mypaquet ]
  \
   | __init__.py
   [ lib ]
     \| __init__.py
      | mymodule.py
```
Les fichiers `__init__.py ` peuvent être vide ou contenir du code. 
