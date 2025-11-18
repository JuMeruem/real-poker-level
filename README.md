# 🃏 Real Poker Level (RPL)

## 📊 Données vivantes

Le classement et les calculs en temps réel sont disponibles ici pour la saison 2025/2026 :
https://docs.google.com/spreadsheets/d/1m1KjRBOiJ22zsFBpwJIQ5gGPUUIRZ3yjNTw_VlZlS3g/edit?usp=sharing

La saison 2024/2025 :
https://docs.google.com/spreadsheets/d/1MQtNq4leYkF_sT8cbul5J_ENsCLTpKpZBdE3VPN9VO0/edit?usp=sharing

La saison 2023/2024 :
https://docs.google.com/spreadsheets/d/1c8bpLM0VNC0MAu11MCxnNkSc-bRh2xo6an52zLIW72o/edit?usp=sharing

---

## Présentation

Le **RPL** (Real Poker Level) est un système de classement inspiré du **ELO des échecs**, spécialement adapté au **poker de club et de tournoi**.  
Il vise à offrir un **classement juste, universel et pédagogique**, reflétant le **niveau réel des joueurs** dans leur environnement.

Créé et développé par **Julien Moal**, ce système est actuellement **testé et validé au PMPC** (Pays de Morlaix Poker Club), où il a montré une convergence rapide et stable des niveaux.

---

## 🎯 Objectif

Créer un classement qui reflète la performance réelle d’un joueur de poker, indépendamment des buy-ins ou des gains financiers.

Le RPL corrige les limites des systèmes existants :

- **Le GPI** dépend des montants investis (et favorise les plus riches)   
- Les adaptations simples du **ELO** ignorent la dynamique multi-joueur des tournois  

---

## ⚙️ Principe général

Chaque joueur est comparé non pas à un seul adversaire, mais à **la moyenne du club ou du tournoi**, comme s’il affrontait à chaque session *“le joueur moyen”*.

- Si le joueur fait mieux que prévu → son RPL augmente  
- S’il fait moins bien → son RPL baisse  
- Plus l’écart entre performance réelle et attendue est grand, plus la variation est forte

Cette approche rend le système **auto-équilibré, progressif et fidèle à la réalité du terrain**.

---

## 📐 Formule complète

**Nouveau_RPL = Ancien_RPL + K × (S − E)**

- **R** : ancien RPL du joueur  
- **K** : constante de progression (32, 24, ou 16 selon le nombre de tournois joués)
- **S** : √(Nb_Joueurs + 1) / Position → score réel selon la place finale
- **E** : 1 / (1 + 10^((RPL_moyen_du_club − Ancien_RPL)/400)) → score attendu selon la moyenne du club

---

## 📊 Exemple d’application

Un tableau d’exemple ainsi qu'un lien google sheets est fourni dans ce dépôt, basé sur les résultats réels du PMPC.  
Il illustre la manière dont le RPL évolue session après session et comment le classement se stabilise avec le temps.

---

## 🧠 Philosophie du RPL

Le RPL n’est pas qu’un chiffre :  
c’est la **trace d’une progression**, la **mesure d’une régularité**, et un **levier de motivation collective**.

> Un joueur qui domine son club verra naturellement son RPL plafonner —  
> c’est normal : pour progresser davantage, il devra affronter des joueurs plus forts.

Ainsi, le système valorise la **mérite réelle** et incite à la **recherche du dépassement**.

---

## 🌍 Diffusion et avenir

Avec une intégration future sur une ou des plateformes en ligne, le RPL pourrait être déployé à grande échelle et devenir **un nouveau standart de classement** d'abord en France et ensuite **la référence du classement poker** partout dans le monde.  

---

## 🧾 Licence

Ce projet est placé sous **licence Creative Commons Attribution - ShareAlike 4.0 International (CC BY-SA 4.0)**.  
Vous pouvez librement le réutiliser, le modifier et le partager à condition de **citer l’auteur** et de **conserver la même licence**.

© 2025 Julien Moal – [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/)
