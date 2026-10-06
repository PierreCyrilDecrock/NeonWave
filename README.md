# Néon Wave

Shoot'em up néon en portrait, installable comme app (PWA) et jouable hors ligne.
Trois modes : Odyssée, Essaim, Convoi.

## Mettre en ligne avec GitHub Pages

1. Crée un dépôt GitHub (public), par exemple `neon-wave`.
2. Envoie tout le contenu de ce dossier **à la racine** du dépôt
   (sur github.com : *Add file → Upload files*, glisse les fichiers et dossiers, y compris `.nojekyll`, puis *Commit*).
3. *Settings → Pages* : *Source* = **Deploy from a branch**, branche **main**, dossier **/ (root)**, puis *Save*.
4. Après environ une minute, le jeu est sur `https://TON-PSEUDO.github.io/neon-wave/`.

## L'ajouter à l'écran d'accueil (iPhone)

1. Ouvre l'adresse dans **Safari**.
2. Touche le bouton *Partager* puis **Sur l'écran d'accueil**, puis *Ajouter*.
3. Lance Néon Wave depuis l'icône : plein écran, sans barre Safari, et ça marche sans réseau.

## Mettre à jour

Remplace les fichiers dans le dépôt. Le service worker (`sw.js`) change de version à chaque modification
de fichier ; l'app se met à jour au lancement suivant (ferme-la complètement puis rouvre-la, parfois deux fois).

## Contenu

- `index.html` : le jeu (un seul fichier, polices incluses à part dans `fonts/`)
- `manifest.webmanifest` : nom, icônes, plein écran portrait
- `sw.js` : cache hors ligne
- `icons/` : icônes (écran d'accueil iOS, Android, favicon)
- `.nojekyll` : demande à GitHub Pages de servir les fichiers tels quels
