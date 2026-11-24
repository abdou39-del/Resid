# 🩺 Résidanat Constantine — Bibliothèque de cours

Site web statique qui transforme le Drive public **« DRIVE DR RAWNEK SAOUDI »**
(https://drive.google.com/drive/folders/1bnCf1RAuFTEUt51kd8eY16oTeOAUM8ns)
en une **bibliothèque organisée, recherchable et présentable**, pensée pour la
présentation du résidanat.

## Utilisation

Ouvrir **`index.html`** dans n'importe quel navigateur (double-clic suffit).
Le dossier doit rester intact (`index.html` + `data.js` ensemble).
Aucun serveur ni connexion n'est requis pour naviguer ; seuls les aperçus et
les liens ouvrent Google Drive (le Drive doit rester public).

## Fonctionnalités

- **Arborescence complète** : Biologie (ANAPATH, Biochimie, Cytologie, Génétique,
  Immuno, Physiologie…), Chirurgie (Gynéco, Ortho, Urgences, Uro, Viscérale),
  Clinique (18 spécialités) — 45 dossiers, 426 fichiers.
- **Recherche instantanée** dans tous les noms de fichiers (insensible aux
  accents), raccourci clavier `/`.
- **Aperçu intégré** d'un cours en un clic (lecteur Drive embarqué), plus
  « Ouvrir dans Drive » et « Télécharger ».
- **Page « Programme officiel »** : correspondance sujet du résidanat ↔ cours
  de l'externat, extraite du PDF officiel, avec lien direct vers le cours
  correspondant quand il existe dans la bibliothèque.
- **Accueil** : 3 piliers, statistiques, aperçu du PDF du programme, fiches
  « ⭐ conseils » par spécialité, fichiers récents.
- Navigation par URL (`#/f/<id-dossier>`), thème clair/sombre, responsive
  (menu latéral coulissant sur mobile).
- **Suivi de progression** (`#/progression`) : coche « ✓ cours fait » et
  « QCM » sur chaque sujet du programme, coche ✓ sur chaque fichier dans
  l'explorateur ; barres de progression globales et par module, filtres
  Tous / À faire / Faits. Enregistré en localStorage (hors ligne, par appareil).

## Fichiers

- `index.html` — application (HTML + CSS + JS, autonome).
- `data.js` — données extraites du Drive (arborescence + programme officiel),
  snapshot du 24/11/2026. Les identifiants Drive permettent des liens directs
  et stables vers chaque fichier/dossier.

## Mise à jour

Si le contenu du Drive change, régénérer `data.js` en réexplorant les dossiers
(les liens `https://drive.google.com/drive/folders/<id>` restent valides).
