# Projet de Classification d'Images: API Flask + Interface Streamlit

Ce projet démontre la création d'une API à l'aide de Flask pour la classification d'images, qui est ensuite intégrée à une interface utilisateur construite avec Streamlit. L'application permet aux utilisateurs de télécharger des images et d'obtenir des prédictions de classification basées sur le modèle entraîné `best_model.h5`.

## Structure du projet

Le projet est structuré comme suit:

```
- backend_api/
   |-- app.py
   |-- best_model.h5
   |-- requirements.txt
   |-- ...
- frontend/
   |-- streamlit_app.py
   |-- requirements.txt
   |-- ...
- README.md
```

### backend_api

Ce dossier contient le serveur backend Flask. Le fichier `app.py` est le point d'entrée de l'API, qui traite les requêtes entrantes, utilise le modèle `best_model.h5` pour prédire la classification de l'image et renvoie la réponse.

### frontend

Contient l'application Streamlit, qui constitue l'interface utilisateur. Les utilisateurs interagissent avec cette interface pour soumettre des images, qui sont ensuite envoyées à l'API Flask via des requêtes HTTP.

## Prérequis

- Python 3.6+
- pip

## Installation

### Configuration de l'environnement

Il est recommandé de créer un environnement virtuel pour éviter les conflits entre les dépendances.

```bash
python -m venv myenv
source myenv/bin/activate  # Sur Windows, utilisez `myenv\Scripts\activate`
```

### Installation des dépendances

Dans les répertoires `frontend` et `backend_api`, installez les dépendances requises avec pip.

```bash
pip install -r requirements.txt
```

Répétez cette étape pour les deux dossiers.

## Utilisation

### Démarrer le serveur backend

Dans le dossier `backend_api`, exécutez la commande suivante pour démarrer le serveur Flask :

```bash
python app.py
```

Cela lancera le serveur backend sur le port par défaut 5000.

### Démarrer l'application frontend

Dans un nouveau terminal, naviguez jusqu'au dossier `frontend` et exécutez la commande suivante :

```bash
streamlit run streamlit_app.py
```

Cela démarrera l'application Streamlit et ouvrira une nouvelle fenêtre dans votre navigateur web par défaut.

## Fonctionnement

Une fois l'application Streamlit lancée, vous pouvez télécharger une image via l'interface utilisateur. Cette image est ensuite envoyée à l'API Flask en backend à l'aide d'une requête HTTP. L'API traite l'image, effectue une prédiction en utilisant le modèle de classification d'images pré-entraîné, et renvoie le résultat à l'interface Streamlit. Les résultats de la prédiction sont ensuite affichés à l'utilisateur.

## Développement et contribution

Les contributions sont ce qui fait de la communauté open source un endroit incroyable pour apprendre, inspirer et créer. Toute contribution que vous apportez est grandement appréciée.

1. Forkez le projet
2. Créez votre branche de fonctionnalités (`git checkout -b feature/AmazingFeature`)
3. Committez vos changements (`git commit -m 'Ajout de quelques AmazingFeature'`)
4. Poussez vers la branche (`git push origin feature/AmazingFeature`)
5. Ouvrez une Pull Request



