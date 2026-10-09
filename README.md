# Powerlifting Log — V1

Application mobile PWA de suivi Powerlifting.

## Inclus
- 660 logs historiques issus du master `Powerlifting_Suivi_Master_2026_MACRO_READY.xlsx`.
- Stockage local navigateur via localStorage.
- Saisie multi-blocs et multi-séries.
- Squat / Bench Press / Deadlift + variantes.
- RPE visé/ressenti par incréments de 0,5.
- Historique, filtres, indicateurs rapides.
- Export JSON `POWERLIFTING_CHATGPT_V1` et CSV.
- Import JSON/CSV.
- Fonctionnement hors connexion après premier chargement.

## Installation téléphone
1. Héberger ce dossier sur un hébergement statique HTTPS (GitHub Pages, Cloudflare Pages, Netlify, etc.).
2. Ouvrir l'URL sur le téléphone.
3. Android Chrome : menu → Ajouter à l'écran d'accueil.
4. iPhone Safari : Partager → Sur l'écran d'accueil.

## Important
Le stockage est local au navigateur/appareil. Faire régulièrement un export JSON. Le JSON est le format recommandé pour transmettre les données à ChatGPT.
