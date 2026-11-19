# Fiche du sujet : CI03 — Prévision de la balance commerciale

**Étudiant :** EL HALLOUFI Saad
**Code Apogée :** 23009160
**Groupe :** CI
**Module :** BD & DS, S7 Commerce international, ENCG Settat, 2026-2027
**Enseignant :** A. Larhlimi

## Sujet (extrait de l'énoncé)
- **Projet :** Prévision de la balance commerciale
- **Question :** prédire le solde commercial par pays
- **Famille :** régression et prévision
- **Modèles conseillés :** Ridge, Random Forest
- **Sources conseillées de l'énoncé :** S5 (Banque mondiale, indicateurs du commerce), S9 (Office des Changes)

## Source des données retenue
- **Nom :** World Development Indicators (WDI)
- **Organisme :** Banque mondiale
- **URL :** https://api.worldbank.org/v2/ (portail : https://data.worldbank.org/topic/trade)
- **Licence :** CC BY 4.0
- **Période et fréquence :** 1995-2023, annuelle
- **Périmètre :** 30 pays, données agrégées de biens et services (sans partenaire ni code SH)
- **Unité d'observation :** un pays pour une année
- **Date d'extraction :** voir data/raw/metadata.json

## Indicateurs utilisés (codes WDI)
| Code | Variable | Unité |
|---|---|---|
| NE.EXP.GNFS.CD | Exportations de biens et services | USD courants |
| NE.IMP.GNFS.CD | Importations de biens et services | USD courants |
| NY.GDP.MKTP.CD | PIB | USD courants |
| NY.GDP.MKTP.KD.ZG | Croissance du PIB réel | % annuel |
| FP.CPI.TOTL.ZG | Inflation (IPC) | % annuel |
| PA.NUS.FCRF | Taux de change officiel | monnaie locale par USD |

## Références
- Banque mondiale, World Development Indicators : https://data.worldbank.org/topic/trade
- Documentation de l'API : https://datahelpdesk.worldbank.org/knowledgebase/topics/125589
- Documentation scikit-learn : https://scikit-learn.org/stable/
