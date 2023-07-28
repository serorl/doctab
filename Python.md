Debut de doc en PYTHON

Sites de référence : 
- (pandas - developpez.com) [https://ghajba.developpez.com/tutoriels/python/introduction-pandas-analyse-donnees/]
- 

# environnement virtuel Venv
- @debian ` apt-get install python3-venv ` installer venv
- @debian `python3 -m venv env & source env/bin/activate ` pour  instancier et activer l'environnement.

# jupyterlab
- pip3 install jupyterlab
- _jupyter lab_  pour lancer jupyter.
- Lancer le notebook dans un répertoire spécifique pour l'accès aux fichiers système.
` jupyter lab --notebook-dir=/home/moi/Documents/  --preferred-dir /home/moi/Documents/DEVWEB/CODEDOC/ `

# pandas & openpyxl
- pip3 install pandas & pip3 install openpyxl ( pour la manimulation des fichiers xls )
- import pandas as pd
- concepts :
    - series : colonne de valeurs  || `myserie = pd.Series([1, 2, 3, 4, 5, 6, 7, 8])` 
    - dataframe : matrice || `df = pd.dataframe()`
- Exemple :
  ``` python
        data = {
            'Pays': ['Russie', 'Italie', 'Maroc', 'France'],
            'Densité': [8.57, 200.27, 65.46, 117.63]
            }
          df = pd.DataFrame( data , index = range(1,5) )
          df.head(3)  # head affiche les premières lignes 
    ```
  
  ``` python
       # lire un fichier
              header = 0 (présence d'un header)
              index_col = None ( ajoute un index )

      df = pd.read_csv('/tmp/TEST.csv', header = 0, index_col = None)
     print( df ) 
  
    ```

  
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
