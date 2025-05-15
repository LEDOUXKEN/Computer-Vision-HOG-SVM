# Pedestrian Detection using HOG and SVM  

**Computer Vision Project | Python | OpenCV | scikit-learn**  

![OpenCV](https://img.shields.io/badge/OpenCV-4.5-%23white?logo=opencv)
![Python](https://img.shields.io/badge/Python-3.8+-blue?logo=python)
![scikit-learn](https://img.shields.io/badge/scikit--learn-1.0+-orange?logo=scikit-learn)

## Description  
Ce projet implémente un système de détection de piétons en utilisant :  
- **HOG (Histogram of Oriented Gradients)** pour l'extraction de caractéristiques.  
- **SVM (Machine à Vecteurs de Support)** comme classifieur.  

L'objectif est d'identifier les piétons dans une image avec une précision optimale, en exploitant des techniques de traitement d'image et de machine learning traditionnel.

## Technologies  
- **Langage** : Python  
- **Bibliothèques** :  
  - `OpenCV` (traitement d'images)  
  - `scikit-learn` (SVM, métriques)  
  - `scikit-image` (extraction HOG)  
  - `NumPy` (calculs matriciels)  
  - `Matplotlib` (visualisation)  

## Fonctionnalités  
- Chargement et prétraitement des images.  
- Extraction des descripteurs HOG.  
- Entraînement d'un modèle SVM linéaire.  
- Évaluation des performances (précision, rappel).  
- Visualisation des résultats avec des bounding boxes.  

## Installation  
1. Clonez le dépôt :  
   ```bash
   git clone https://github.com/votre-utilisateur/pedestrian-detection.git
   cd pedestrian-detection

 2.Installez les dépendances : 
 pip install opencv-python scikit-learn scikit-image numpy matplotlib

 Utilisation
Exécutez le script principal :

bash
python main.py --image_path data/test_image.jpg
Arguments optionnels :

--model_path : Chemin vers un modèle pré-entraîné (par défaut : models/svm_model.pkl).

--visualize : Affiche les résultats (par défaut : True).

Résultats
Exemple de détection :
Résultat

Métriques :
Précision 	Rappel	F1-Score
92%	         88%	    90%

Structure du projet
pedestrian-detection/  
├── data/                  # Images de test  
├── models/                # Modèles sauvegardés  
├── results/               # Visualisations des résultats  
├── src/  
│   ├── hog_extraction.py  # Extraction HOG  
│   ├── train_svm.py       # Entraînement SVM  
│   └── detect.py          # Détection sur nouvelles images  
├── main.py                # Script principal  
└── README.md  

Améliorations futures:
_Intégration de YOLO/Faster R-CNN pour une détection en temps réel.
_Optimisation des paramètres HOG/SVM via grid search.
_Application à des flux vidéo (OpenCV VideoCapture).

Contribution
Les contributions sont les bienvenues ! Ouvrez une issue ou soumettez une pull request.

Licence
Ce projet est sous licence MIT. Voir le fichier LICENSE.

