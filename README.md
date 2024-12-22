# Simulation Chirurgicale et Reconstruction 3D avec 3D Slicer

## Description du Projet
Ce projet est une extension pour 3D Slicer visant à améliorer l'apprentissage des étudiants en chirurgie à travers des simulations 3D interactives et la reconstruction volumétrique à partir de fichiers DICOM. Il se compose de trois modules principaux :

1. **SurgicalSimulation** : Permet des simulations chirurgicales avec des outils interactifs de manipulation et de seuil.
2. **Reconstruction3D** : Fournit des outils pour créer et analyser des reconstructions 3D à partir de volumes DICOM.
3. **DICOMLoader** : Simplifie le chargement et l’affichage des fichiers DICOM dans 3D Slicer.

## Fonctionnalités Principales
### 1. **SurgicalSimulation**
- Simulation chirurgicale interactive basée sur des données volumétriques.
- Fonctionnalités de seuil et d’inversion pour isoler des structures spécifiques.
- Intégration avec des volumes scalaires pour une analyse précise.

### 2. **Reconstruction3D**
- Reconstruction 3D à partir de fichiers DICOM.
- Analyse des volumes reconstruits avec des outils d’inspection.
- Supporte les formats NRRD et DICOM.

### 3. **DICOMLoader**
- Chargement rapide de fichiers DICOM via une interface utilisateur intuitive.
- Affichage des volumes chargés dans la scène de 3D Slicer.
- Notifications d’erreurs claires en cas de problèmes de chargement.

## Prérequis
Avant d'utiliser ce projet, assurez-vous d'avoir installé :

- **3D Slicer** : Version 5.0 ou ultérieure ([téléchargeable ici](https://www.slicer.org/)).
- **Python** : Les dépendances sont automatiquement gérées par 3D Slicer.

## Installation
1. Clonez ce dépôt sur votre machine locale :
   ```bash
   git clone https://github.com/majdsaadouli/Simulation-Chirurgicale-et-Reconstruction-3D-avec-3D-Slicer.git
   ```

2. Copiez les fichiers Python dans le dossier des modules de votre installation 3D Slicer :
   ```bash
   cp *.py $HOME/.config/NA-MIC/Extensions-<version>/Slicer/Modules/.
   ```

3. Redémarrez 3D Slicer pour charger les modules.

## Utilisation
### 1. **Chargement de Fichiers DICOM**
- Accédez au module **DICOMLoader** dans l’interface de 3D Slicer.
- Cliquez sur "Charger une image DICOM" et sélectionnez votre fichier.

### 2. **Simulation Chirurgicale**
- Accédez au module **SurgicalSimulation**.
- Sélectionnez un volume d’entrée et ajustez les paramètres de seuil pour isoler des structures.
- Visualisez les résultats en temps réel dans la scène 3D.

### 3. **Reconstruction 3D**
- Accédez au module **Reconstruction3D**.
- Chargez un volume DICOM et utilisez les outils fournis pour créer une reconstruction 3D.
- Appliquez des seuils pour analyser les structures internes.

## Structure des Fichiers
- `SurgicalSimulation.py` : Contient le module de simulation chirurgicale.
- `Reconstruction3D.py` : Contient le module de reconstruction 3D.
- `DICOMLoader.py` : Permet le chargement de fichiers DICOM.

## Exemples de Cas d'Utilisation
### Exemple 1 : Simulation d'une Chirurgie de la Colonne Vertébrale
1. Chargez un fichier DICOM d’une colonne vertébrale.
2. Appliquez un seuil pour isoler les vertèbres.
3. Simulez des coupes chirurgicales interactives.

### Exemple 2 : Reconstruction d'un Modèle 3D
1. Chargez un ensemble de fichiers DICOM d’un scanner.
2. Utilisez le module **Reconstruction3D** pour créer un modèle 3D.
3. Exportez le modèle pour une impression 3D.

## Limitations
- Fonctionne uniquement avec des fichiers DICOM valides.
- Les performances peuvent être réduites pour des ensembles de données volumineux.

## Améliorations Futures
- Ajouter un outil de segmentation automatique basé sur l'apprentissage automatique.
- Intégrer un export direct vers des logiciels de CAO.
- Améliorer l’interface utilisateur pour plus d’accessibilité.

## Contribuer
Les contributions sont les bienvenues !
1. Forkez ce dépôt.
2. Créez une branche pour vos modifications :
   ```bash
   git checkout -b nouvelle-fonctionnalite
   ```
3. Soumettez une pull request.

## Auteurs
- **Majd Saadouli (https://github.com/majdsaadouli/)** : Étudiant en génie biomédical et développeur passionné par les technologies médicales.


---
Merci d'utiliser cette extension pour 3D Slicer ! N’hésitez pas à partager vos retours et suggestions.

