
# Projet de Gestion de Réservations et Clients

Ce projet Python/SQLite est conçu pour gérer une base de données permettant la gestion des clients et des réservations. Il utilise SQLite pour le stockage des données et Python pour les interactions et manipulations via des scripts.

## Fonctionnalités Principales

1. **Gestion des clients** : Ajout, suppression et mise à jour des informations des clients.
2. **Gestion des réservations** : Création, suppression et affichage des réservations associées aux clients.
3. **Base de données robuste** : Utilisation de SQLite pour gérer efficacement les relations entre les entités.

## Prérequis et Installation

### Windows

1. Téléchargez et installez Python 3 à partir du site officiel :
   - [Python 3.9.2 - 64 bits](https://www.python.org/ftp/python/3.9.2/python-3.9.2-amd64.exe)
   - [Python 3.9.2 - 32 bits](https://www.python.org/ftp/python/3.9.2/python-3.9.2.exe)
2. Pendant l'installation, cochez l'option **"Add Python to PATH"**.

### Linux

1. Ouvrez un terminal et installez Python avec SQLite :
   ```bash
   sudo apt install -y python3 libsqlite3-dev
   ```
2. Installez les dépendances nécessaires avec pip :
   ```bash
   pip install --user -r requirements.txt
   ```

## Utilisation

### Mode Console

1. Lancez le fichier principal `main.py` :
   - Sous Linux :
     ```bash
     python3 main.py
     ```
   - Sous Windows :
     ```bash
     py main.py
     ```
2. Naviguez dans le menu principal pour gérer les clients et les réservations.

### Mode Interactif

Vous pouvez interagir directement avec la base de données pour effectuer des requêtes spécifiques. Exemple :

```python
$ python3
>>> from utils import db
>>> conn = db.creer_connexion("data/voile.db")
>>> db.supprimer_client(conn, 101)  # Exemple : supprimer un client par numéro
```

### Utilisation avec un IDE

Pour un développement plus confortable, utilisez un IDE comme **PyCharm**. Configurez-le pour exécuter `main.py` et utilisez les outils intégrés pour le débogage et l'exécution.


