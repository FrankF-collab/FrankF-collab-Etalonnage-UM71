# Application Mesures

Application web mobile de saisie de mesures (fiches, calcul KCA / bornes) avec import et export Excel (`.xlsx`).
Un seul fichier HTML, sans dépendance ni serveur : tout fonctionne dans le navigateur.

## Utilisation

Ouvrir la page publiée : `https://<utilisateur>.github.io/<depot>/`

Sur téléphone, l'ajouter à l'écran d'accueil (menu du navigateur → « Ajouter à l'écran d'accueil »).

## Fonctionnalités

- Saisie par onglets, enregistrement de plusieurs fiches
- Calcul automatique (KCA, ponts, recherche de solutions)
- Import / export de classeurs Excel `.xlsx`
- Envoi par e-mail du fichier exporté (via `mailto:`)
- Thème clair / sombre automatique

## Données

Les données restent **uniquement dans votre navigateur** (`localStorage` et `IndexedDB`). Rien n'est envoyé à un serveur.
Elles sont propres à chaque appareil et navigateur : pensez à exporter régulièrement vos fiches en Excel.

## Publier sur GitHub Pages

1. Créer un dépôt et y déposer `index.html`, `.nojekyll` et `README.md`
2. **Settings → Pages → Build and deployment** : *Deploy from a branch*, branche `main`, dossier `/ (root)`
3. L'application est en ligne après une minute environ

## Développement local

Ouvrir `index.html` dans un navigateur, ou lancer un serveur local :

```bash
python3 -m http.server 8000
```
