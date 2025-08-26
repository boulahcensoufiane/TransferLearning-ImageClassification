[README.md](https://github.com/user-attachments/files/21992501/README.md)
# 🖼️ Apprentissage par transfert pour la classification d’images  

## 📌 Description
Classification d’images par **apprentissage par transfert (Transfer Learning)** avec plusieurs architectures CNN et Transformers modernes.  
Les modèles implémentés sont : **VGG19, ResNet34, DenseNet121, EfficientNet et Vision Transformer (ViT)**.  
Le dataset utilisé est **PlanetVillage** (ou un dataset similaire organisé en dossiers).  

---

## 📂 Structure du projet
```
TP-TransferLearning-ImageClassification/
│── data/                   # Dataset (train/val/test)
│── notebooks/              # Notebooks Jupyter pour chaque exercice
│   ├── exo1_models.ipynb
│   ├── exo2_pretrained.ipynb
│   ├── exo3_efficientnet_vit.ipynb
│── src/                    
│   ├── dataset.py          # Prétraitement & DataLoader
│   ├── train.py            # Boucle d’entraînement générique
│   ├── utils.py            # Fonctions utilitaires (graphiques, métriques)
│── results/                # Sauvegarde des modèles et courbes
│── README.md               # Documentation
```

---

## 🚀 Installation
1. Cloner le dépôt :
```bash
git clone https://github.com/ton-utilisateur/TP-TransferLearning-ImageClassification.git
cd TP-TransferLearning-ImageClassification
```

2. Créer un environnement virtuel et installer les dépendances :
```bash
pip install -r requirements.txt
```

---
## 📊 Expérimentations
### 🔹 Exercice 1 : Modèles de base
- VGG19, ResNet34, DenseNet121 sans pré-entraînement.  

### 🔹 Exercice 2 : Poids pré-entraînés (ImageNet)
- Réutilisation des modèles avec `weights=ImageNet`.  
- Remplacement de la tête de classification.  

### 🔹 Exercice 3 : EfficientNet & ViT
- Application du transfert learning avec EfficientNet-B0 et ViT-B/16.  

---

## 📈 Résultats attendus
- Courbes **loss / accuracy** (entraînement et validation).  
- Comparaison des modèles en termes de précision, rapidité, et taille.  

---

## 📚 Références
- He et al. (ResNet): [arXiv:1512.03385](https://arxiv.org/pdf/1512.03385.pdf)  
- Huang et al. (DenseNet): [Springer](https://link.springer.com/chapter/10.1007/978-3-030-51935-3_7)  
- Tan & Le (EfficientNet): [arXiv:1905.11946](https://arxiv.org/pdf/1905.11946.pdf)  
- Dosovitskiy et al. (ViT): [arXiv:2010.11929](https://arxiv.org/pdf/2010.11929.pdf)  
