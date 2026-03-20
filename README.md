# Traintesters

## Description du Projet

Ce projet explore comment les idiomes sont traités et interprétés à l'intérieur des modèles de langage de type Transformer.

Le projet analyse le traitement des idiomes dans différents contextes linguistiques et à travers diverses architectures de modèles de langage, en se concentrant sur la compréhension figurative versus littérale.

## Langues et Idiomes Étudiés

- **Français** : Idiomes français courants
- **Anglais** : Idiomes anglais
- **Chinois** : Idiomes chinois
- **Arabe** : Idiomes arabes
- **Langues turciques** : Azerbaïdjanais, turc, ouzbek

## Méthodologies d'Analyse

### 1. Analyse d'Embeddings
- Génération d'embeddings multilingues avec des modèles comme MiniLM-L12, BGE-M3
- Réduction de dimension (UMAP) pour visualisation 2D
- Comparaison de similarités cosinus entre interprétations littérales et figuratives

### 2. Analyse d'Attention
- Étude des mécanismes d'attention dans les modèles Transformer
- Visualisation des poids d'attention pour comprendre comment les modèles traitent les idiomes
- Comparaison entre modèles encodeur-only (BERT, DistilBERT) et décodeur-only (Qwen)

### 3. Évaluation LLM
- Utilisation de modèles comme Qwen pour évaluer la qualité des traductions d'idiomes
- Classification des traductions selon des catégories (bonne traduction, traduction littérale, erreur de traduction, etc.)
- Analyse de similarité sémantique entre différentes interprétations

### 4. Analyse de Similarité
- Calcul de scores de similarité entre variantes d'idiomes
- Clustering et visualisation des relations sémantiques
- Comparaison inter-langues des patterns d'idiomes

## Modèles Utilisés

- **Encodeurs** :
  - BERT multilingue (bert-base-multilingual-cased)
  - DistilBERT multilingue (distilbert-base-multilingual-cased)
  - MiniLM-L12 (sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2)
  - BGE-M3 (BAAI/bge-m3)

- **Décodeurs** :
  - Qwen2.5 (1.5B, 7B, 0.5B)
  - Llama 3.1

### Méthodes externes
- Ollama (pour l'inférence locale avec Qwen/Llama)

## Utilisation

Chaque notebook Jupyter peut être exécuté indépendamment. Commencer par :

## Résultats et Visualisations

Le projet génère diverses visualisations :
- Projections 2D d'embeddings d'idiomes
- Matrices d'attention
- Graphiques de similarité
- Analyses de clustering

Les résultats sont sauvegardés dans des fichiers CSV pour analyse ultérieure.

## Licence

Ce projet est sous licence MIT.