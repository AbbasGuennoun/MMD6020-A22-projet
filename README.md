# MMD6020-A22-projet
- Repo du projet de cours : MMD6020 (médecine computationnelle)
- Université de Montréal, Québec 

# Description : 

## Titre du projet : 

An ecologically motivated approach to prompt engineering for zero-shot image classification with CLIP

## Rationnelle du projet : 

- Les processus cognitifs de l'Homme sont controlés par des mécanismes complexes faisant intervenir plusieurs composantes du cerveau permettant la mise en place de schémas psychologiques qui permettent l'analyse et l'interprétation de nouvelles informations.
- Le perceptron, unité de base des réseaux de neurones artificiels, est un modèle mathématique initialement inspiré de fonctionnement du neurone humain. Les réseaux de neurones artificiels sont très performants pour la tâche pour laquelle ils ont été entrainés, mais leurs performances baissent dès qu'on dévie de cette tâche. 
- L'avènement de réseaux de neurones multimodaux, capables de faire de la reconnaissance en combinant des images et du texte, se rapprocherait des représentations "de haut niveau" des humains.  

## Question de recherche : 

Le but de ce projet est d’employer une banque de stimuli visuels accompagnée de variables psycholinguistiques pour comparer les schémas humains aux représentations de haut niveau développées par CLIP. L’utilisation de telles variables limite les décisions arbitraires et permet d’informer le prompt engineering avec des données écologiquement valides. Spécifiquement, nous voulons savoir si un réseau multimodal, comme CLIP, peut être lié à des données humaines pour aller plus loin que la simple reconnaissance d’objet et interroger des schémas complexes, notamment le dégoût, de manière fiable. 


# Méthodologie 

## Modèle utilisé : CLIP 

- CLIP (Contrastive Language–Image Pre-training, développé par OpenAI) est un réseau de neurone multimodal capable d'apprendre des concepts visuels à partir de texte. Cette particularité permet la généralisation de ces modèles, qui sont capables de reconnaitre un concept visuel qui n'ont encore jamais vu à partir la description de ce dernier. 

- Ce modèle a entrainé sur des millions d'images accoompangées de texte, et utilisant plusieurs techniques à savoir : le zero-shot transfer, le 'natural language supervision', et l'apprentissage multimodal.

Article décrivant le développement de CLIP : https://arxiv.org/abs/2103.00020

Code CLIP (GitHub) : https://github.com/openai/CLIP

## Base de données : DIRTI

- Pour comparer les représentations de 'haut niveau' de CLIP et de la cognition humaines, nous avons utilisé une base de données en open-access d'images spécialement préparée pour stimuler l'émotion du 'dégout', et qui a été mise à diposition des chercheurs étudiant cette émotion. (https://zenodo.org/record/167037#.Y4vcM-zMLOQ)

## Schéma du pipeline du projet : 

![méthode](https://github.com/AbbasGuennoun/MMD6020-A22-projet/blob/main/Figures/Pipeline.png)

## Notre étude : 

### Notebook : 

- La version 1 : Premiers essais des modèles avec les premières visualisations, pre-processing des images, et visualisations de la base de données

- La version 2 : Réduction de la dimensionnalité UMAP (Uniform Manifold and Projection), entraînement du modèle de comparaison et visualisation du nombre de K optimal en fonction de la perte. 

- La version 3 : Métriques de performances des 4 modèles (baseline et modèles écologiquement motivés), courbes ROC, nettoyage des autres parties du code

### Résumé : 

Le projet comporte deux phases : 

- Une première phase constituant la "BASELINE" de l'étude où on a testé CLIP (modèle pré-entraîné) et entraîné le modèle KNN de comparaison afin d'avoir une base de comparaison lorsque les modèles sont écologiquement motivées. 

- Une deuxième phase où les deux modèles sont écologiquement motivés (ajout d'une variable psycholinguistique au niveau des textes utilisés)

A noter qu'avant l'entame des deux phases, les images ainsi que les textes ont été encodés avec CLIP (voir schéma pipeline)

### Article (écrit pour le cours) : 

- Présentation de la rationnelle de l'étude 
- Explication de la méthodologie 
- Exposition des résultats 
- Discussion des résultats 
- Perspectives d'avenir

![méthode](https://github.com/AbbasGuennoun/MMD6020-A22-projet/blob/main/Figures/Article2.png)

# Installation

- L'ensemble des libraires et modules nécessaires au fonctionnement et à l'éxecution du Notebook sont sur le fichier requirements.txt 
- Pour plus d'informations sur CLIP et son utilisation, veuillez consulter le repo GitHub des auteurs (informations sur le readme) : https://github.com/openai/CLIP#readme

# Auteurs 

- Shawn Manuel
- Abbas Guennoun

# Références : 

- Référence pértinente d'un blogpost autour de CLIP : https://medium.com/mlearning-ai/having-fun-with-clip-features-part-i-29dff92bbbcd



