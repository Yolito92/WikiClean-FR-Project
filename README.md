
# 🇫🇷 Zeronex – Wikipedia FR Clean Dataset (Extrait )
### Démonstration de nettoyage, normalisation et structuration d’un corpus massif

Ce dépôt contient **un extrait représentatif (~0.0001)** du travail réalisé sur le dump complet de Wikipédia FR.  
Cet extrait a pour but de **montrer la qualité du nettoyage**, la cohérence du format final et l’exploitabilité immédiate pour les applications IA (NLP, RAG, embeddings, graph databases…).

Le dataset complet comprend **2,7 millions d’articles**, mais seule une fraction est publiée ici.

---

## 🧠 Objectif du projet

Transformer le contenu brut de Wikipédia FR, naturellement complexe et peu exploitable, en un dataset :

- propre  
- stable  
- homogène  
- lisible  
- structurellement cohérent  
- prêt à être utilisé dans n’importe quel pipeline IA

L’extrait inclus démontre la capacité à :

- nettoyer et normaliser le texte (suppression du wikitext, HTML, templates inutiles…)  
- restructurer les infobox en paires clé/valeur  
- isoler proprement les références  
- extraire les liens internes  
- organiser les catégories  
- produire un JSON clair, portable et réutilisable  

---

## 📊 Contenu de l’extrait (~10%)

Chaque fichier JSON présent dans ce dépôt suit une structure stable contenant :

- **title** — titre de l’article  
- **text_clean** — texte principal nettoyé  
- **infobox** — informations structurées lorsqu’elles existent  
- **links** — liens internes extraits  
- **references** — références externes isolées  
- **categories** — catégories d’origine  
- **timestamp** — date de révision  
- **revision_id** — identifiant de la révision  

Cet extrait est fourni **exclusivement pour illustrer l’efficacité du processus**.

---

## 🟪 Pourquoi seulement 10% ?

Ce repository ne vise pas à redistribuer la totalité du dump Wikipédia FR, mais à :

- présenter la **méthode de transformation**  
- montrer la **qualité du nettoyage**  
- démontrer la **stabilité du format**  
- fournir une **preuve de concept exploitable**  
- permettre des tests réels sur une partie représentative du corpus  

Le dataset complet (2,7M articles) dépasse le cadre d’une release GitHub classique.

---

## 🌍 Usages possibles de l’extrait

Cet extrait permet déjà de tester :

- pipelines NLP  
- modèles RAG  
- moteurs de recherche  
- embeddings  
- extraction d’entités (NER)  
- bases de graphes  
- indexation full-text  
- QA systems en français  

Sans nécessiter le dataset complet.

---

## 🧩 Philosophie

Rendre le savoir francophone plus accessible aux systèmes modernes d’IA en proposant un format :

- épuré  
- standardisé  
- polyvalent  
- immédiatement utilisable  

Ce projet s’inscrit dans une démarche d’ouverture, de clarté et d’amélioration continue.

---

## 📦 Format du dataset (extrait)

Chaque fichier suit la structure :

```json
{
  "title": "",
  "text_clean": "",
  "infobox": {},
  "links": [],
  "references": [],
  "categories": [],
  "timestamp": "",
  "revision_id": ""
}
