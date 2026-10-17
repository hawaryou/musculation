# Training OS — Musculation

Carnet d'entraînement mobile-first en HTML/CSS/JavaScript, sans serveur ni dépendance de build.

## Fonctionnalités
- Planning hebdomadaire : badminton lundi/jeudi, musculation mardi/mercredi/vendredi et séance complémentaire facultative le week-end.
- Exercices préremplis avec séries, répétitions, charge cible, tempo, repos et consignes.
- Saisie de la charge réelle, des répétitions et du RIR, avec validation série par série.
- Historique, volume d'entraînement, graphique de progression et suivi du poids corporel.
- Notes de séance et suivi du sommeil/fatigue.
- Bilan hebdomadaire à copier dans ChatGPT pour analyse et préparation de la semaine suivante.
- Export/import JSON des données et cache hors-ligne basique (PWA).

## Lancer
Ouvre `index.html` dans un navigateur. Pour tester le service worker/PWA, utilise un serveur local, par exemple `python -m http.server 8000`, puis ouvre `http://localhost:8000`.

## Publier avec GitHub Pages
1. Ouvre **Settings → Pages**.
2. Choisis **Deploy from a branch**, branche `main`, dossier `/ (root)`, puis enregistre.
3. Après le déploiement, l'application sera généralement accessible à `https://hawaryou.github.io/musculation/`.

## Données et limites
Les performances sont stockées dans le `localStorage` du navigateur de l'appareil et ne se synchronisent pas automatiquement entre appareils. Exporte régulièrement une sauvegarde JSON. Le bilan hebdomadaire prépare un texte pour ChatGPT, mais n'appelle pas automatiquement une IA. Les charges sont indicatives : adapte-les à la machine, à la technique et à la récupération.
