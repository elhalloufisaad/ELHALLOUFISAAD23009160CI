# CI03 — Prévision de la balance commerciale

Contrôle continu, Partie B : Machine Learning appliqué au commerce international.
ENCG Settat · S7 Commerce international · Module BD & DS · 2026-2027 · Enseignant : A. Larhlimi

## Identité
- **Étudiant :** EL HALLOUFI Saad
- **Code Apogée :** 23009160
- **Groupe :** CI
- **Sujet attribué :** CI03 — Prévision de la balance commerciale

## Objectif
Prévoir le solde commercial d'un pays (en % du PIB) à partir de données macroéconomiques, avec une comparaison à une référence naïve et une validation sans fuite de données.

## Données
- **Source :** Banque mondiale, World Development Indicators (WDI) — https://api.worldbank.org/v2/
- **Licence :** CC BY 4.0
- **Période :** 1995-2023, fréquence annuelle, 30 pays
- **Récupération :** script `data/raw/telecharger_donnees.py` (produit `wdi_ci03.csv` et `metadata.json`)

## Structure du dépôt
```
├── README.md
├── requirements.txt
├── .gitignore
├── DECLARATION_IA.md
├── data/raw/            # script de téléchargement et données
├── docs/                # fiche du sujet (fiche_CI03.md)
├── notebooks/           # projet_CI03.ipynb
├── figures/             # graphiques en couleurs
└── rapport/             # export PDF du notebook (rapport.pdf)
```
Les dossiers `presentation/` et `video/` seront ajoutés lors de la séance prévue pour ces livrables.

## Exécution
1. Installer les dépendances : `pip install -r requirements.txt`
2. Télécharger les données : `python data/raw/telecharger_donnees.py`
3. Ouvrir `notebooks/projet_CI03.ipynb` (Jupyter ou Google Colab) et exécuter les cellules dans l'ordre.

Dans Google Colab :
```
!git clone https://github.com/elhalloufisaad/ELHALLOUFISAAD23009160CI.git
%cd ELHALLOUFISAAD23009160CI
!pip install -r requirements.txt
!python data/raw/telecharger_donnees.py
```

## Reproductibilité
- Graine aléatoire fixée à 42.
- Chemins relatifs, aucune clé d'API ni donnée confidentielle.
- Usage des outils d'IA déclaré dans `DECLARATION_IA.md`.
