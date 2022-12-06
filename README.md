# MMD6020-A22-projet
- Repo du projet de cours : MMD6020 (médecine computationnelle)
- Université de Montréal, Québec 

# Description : 

## Titre du projet : 

Cross-modal comparison of high-level representations: an ecologically motivated approach to prompt engineering for zero-shot image classification within a multimodal network

## Rationnel du projet : 

- Les processus cognitifs de l'Homme sont controlés par des mécanismes complexes faisant intervenir plusieurs composantes du cerveau permettant la mise en place de schémas psychologiques qui permettent l'analyse et l'interprétation de nouvelles informations.
- Le perceptron, unité de base des réseaux de neurones artificiels, est un modèle mathématique initialement inspiré de fonctionnement du neurone humain. Les réseaux de neurones artificiels sont très performants pour la tâche pour laquelle ils ont été entrainés, mais leurs performances baissent dès qu'on dévie de cette tâche. 
- L'avènement de réseaux de neurones multimodaux, capables de faire de la reconnaissance en combinant des images et du texte, se rapprocherait des représentations "de haut niveau" des humains.  

## Questions de recherche : 

- Comparer les schémas cognitifs des humains aux représentations de 'haut niveau' ces réseaux de neurones, et notamment les schémas à l’origine du développement de l’émotion chez l’Homme, en employant des banques de stimuli visuels, accompagnées de variables psychologiques

- Est ce que l'utilisation d'un réseau multimodal permetterait d'aller plus loin que la simple reconnaissance d’objet?

# Méthodologie 

## Modèle utilisé : CLIP 

- CLIP (Contrastive Language–Image Pre-training, développé par OpenAI) est un réseau de neurone multimodal capable d'apprendre des concepts visuels à partir de texte. Cette particularité permet la généralisation de ces modèles, qui sont capables de reconnaitre un concept visuel qui n'ont encore jamais vu à partir la description de ce dernier. 

- Ce modèle a entrainé sur des millions d'images accoompangées de texte, et utilisant plusieurs techniques à savoir : le zero-shot transfer, le 'natural language supervision', et l'apprentissage multimodal.

Article décrivant le développement de CLIP : https://arxiv.org/abs/2103.00020

Code CLIP (GitHub) : https://github.com/openai/CLIP

## Base de données : DIRTI

- Pour comparer les représentations de 'haut niveau' de CLIP et de la cognition humaines, nous avons utilisé une base de données en open-access d'images spécialement préparée pour stimuler l'émotion du 'dégout', et qui a été mise à diposition des chercheurs étudiant cette émotion. (https://zenodo.org/record/167037#.Y4vcM-zMLOQ)

## Notre étude : 

- Notebook : Le fichier Notebooks contient les différentes étapes du projet, ainsi que les différentes visualisations. Vous y trouverez également des explications supplémentaires. 
- Article (écrit pour le cours) : 

# Installation

- L'ensemble des libraires et modules nécessaires au fonctionnement et à l'éxecution du Notebook sont sur le fichier requirements.txt 
- Pour plus d'informations sur CLIP et son utilisation, veuillez consulter le repo GitHub des auteurs (informations sur le readme) : https://github.com/openai/CLIP#readme

# Auteurs 

- Shawn Manuel
- Abbas Guennoun

# Références : 

- Référence pértinente : https://medium.com/mlearning-ai/having-fun-with-clip-features-part-i-29dff92bbbcd



