# 🗑️ Neovision - Classification des Déchets avec l'IA

## 📖 Présentation du Projet
L’augmentation des déchets et les défis liés au recyclage nécessitent des solutions innovantes. Ce projet repose sur **l’intelligence artificielle** et les **réseaux de neurones convolutifs (CNN)** pour **classer automatiquement les déchets** à partir d’images.

📌 **Objectif** : Développer un modèle IA permettant de **classifier les déchets** en plusieurs catégories avec **85 % de précision** et un **temps d’inférence optimal**.

## 🚀 Fonctionnalités Clés
✅ **Classification automatique des déchets** grâce à un modèle CNN  
✅ **85% de précision** sur les données de test  
✅ **Temps d’inférence rapide** 
✅ **Techniques avancées de Data Augmentation** pour améliorer les performances  
✅ **Utilisation de TensorFlow et Keras** pour l’entraînement du modèle  

## 📂 Contenu du Dépôt
- `Tri_Intelligent_IA.ipynb` : Notebook principal contenant tout le code du projet


## 📊 Prétraitement des Données
Les données doivent être fournies par l'utilisateur et chargées dans le notebook.  
Le modèle est conçu pour fonctionner avec un jeu de données structuré en images et labels.

## 🔄 Augmentation et Préparation des Données
Pour améliorer les performances du modèle, différentes techniques d’augmentation des données sont appliquées :
- **Rotation aléatoire** des images.
- **Inversion horizontale et verticale**.
- **Ajustement de la luminosité**.
- **Translation et décalage des images**.
- **Redimensionnement des images en 64x64**.
- **Normalisation des valeurs des pixels**.

Chaque catégorie de déchets est augmentée de manière dynamique afin d’équilibrer le dataset et éviter le surapprentissage.

## 🏗️ Construction du Modèle CNN
Le modèle est construit avec plusieurs couches convolutives :
- **4 couches de convolution** avec **filtres 3x3**, activation **ReLU**, suivies de **MaxPooling 2x2**.
- **Batch Normalization** et **Dropout (0.25)** pour éviter le surapprentissage.
- **Une couche Flatten** pour transformer les caractéristiques en vecteur avant la classification.
- **Une couche Dense de 512 neurones** avec activation ReLU.
- **Dropout (0.5)** après la couche Dense pour améliorer la généralisation.
- **19 classes de sortie** avec activation **softmax**.

L’optimisation du modèle est réalisée avec :
- **Fonction de perte** : categorical cross-entropy.
- **Optimiseur** : Adam avec un taux d’apprentissage de **0.001**.
- **50 époques d’entraînement** avec batch de **250 images**.
- 

## 📊 Évaluation et Résultats
- **Amélioration progressive de la précision** au fil des époques.
- **Validation Loss :**
  - Diminue de **3.79** à **0.43** au fil des époques.
- **Test Accuracy finale** : **87.3%**
- **Exemple de prédiction réussie** sur une image testée en temps réel.

## 🛠 Technologies Utilisées
- **Python** (TensorFlow, Keras, OpenCV, Matplotlib, Scikit-learn)
- **Deep Learning** (CNN, Data Augmentation)
- **Jupyter Notebook** pour l’expérimentation

## 📧 Contact
Si vous avez des questions ou suggestions, n’hésitez pas à me contacter via mon profil GitHub.
