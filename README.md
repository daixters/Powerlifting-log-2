# Powerlifting — suivi adaptatif (GitHub Pages)

## Mettre à jour le site existant
1. Télécharge/exporte une sauvegarde JSON de l'application actuelle si elle contient des logs. Garde aussi une copie des anciens fichiers GitHub.
2. Décompresse cette archive.
3. Dans le dépôt GitHub actuel, choisis `Add file` → `Upload files` et téléverse `index.html`, `manifest.webmanifest` et `sw.js` à la racine (au même niveau que l'ancien `index.html`).
4. Commit les changements. GitHub Pages republie normalement le site à la même URL ; ne crée pas de nouveau dépôt.
5. Ouvre le site sur le téléphone. Si l'ancienne version reste affichée, ferme l'onglet, rouvre-le et actualise ; au besoin, vide le cache du site.

## Import de l'historique
Dans l'onglet Données, importe le JSON exporté de l'ancienne app ou un CSV. Les JSON attendus peuvent être un tableau ou un objet avec `logs`, `LOGS`, `history`, `data` ou `entries`. Les CSV doivent avoir des en-têtes de type Date, Exercice/Mouvement, Variante, Charge/Charge (kg), Reps, Séries, RPE/RPE ressenti, RPE visé et Commentaire. Vérifie le nombre de lignes après import et conserve la sauvegarde originale.

## Stockage et calculs
Les données sont stockées dans le `localStorage` du navigateur et ne sont pas synchronisées automatiquement entre appareils. Exporte régulièrement le JSON. Ne mets jamais l'historique personnel dans le dépôt public.

Volume = kg × reps × séries. Intensité relative = charge / référence configurable × 100. Les références par défaut sont squat 190 kg, bench 155 kg et deadlift 240 kg ; modifie-les si nécessaire. Les recommandations sont heuristiques, pas un score physiologique validé. Les comparaisons de fatigue restent prudentes et doivent être interprétées avec sommeil, douleurs, stress et contexte. Pas de vitesse ni de vélocité.
