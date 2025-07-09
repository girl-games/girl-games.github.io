# Girl Games – GitHub Pages

Ce dossier contient un site vitrine simple pour héberger des jeux via des iframes sur **GitHub Pages**.

## Structure
```
girl-games-site/
├── index.html   # page d’accueil
├── style.css    # styles simples et responsives
├── script.js    # script minimal
└── README.md
```

## Ajouter ou remplacer des jeux
- Localisez la section `<iframe>` dans `index.html`.
- Remplacez l’URL par celle d’un jeu **autorisé à être embarqué** (`X-Frame-Options` doit être permissif).
- Ajoutez ou dupliquez des `<article class="game-card">` pour plus de jeux.

## Mise en ligne sur https://girl-games.github.io/

1. Créez ou connectez-vous à un compte GitHub portant le nom d’utilisateur **girl-games** *(ou changez l’URL ci‑dessus si vous avez un nom différent)*.
2. Dans ce compte, créez un **nouveau dépôt public** appelé **girl-games.github.io** – l’orthographe doit être exactement `username.github.io` pour un site utilisateur.
3. Téléversez tout le contenu de ce dossier (ou décompressez l’archive) à la racine du dépôt.
   - Via l’interface web, bouton **Add files → Upload files**.
   - Ou en ligne de commande :
     ```bash
     git clone https://github.com/girl-games/girl-games.github.io.git
     cd girl-games.github.io
     # Copiez vos fichiers dans ce répertoire
     git add .
     git commit -m "Initial commit of Girl Games site"
     git push origin main
     ```
4. Patientez quelques secondes : GitHub Pages construit automatiquement le site.  
   L’adresse sera **https://girl-games.github.io/**.
5. Videz le cache/rafraîchissez votre navigateur pour voir le résultat.

### Conseils
- GitHub Pages sert uniquement des fichiers statiques.  
  Aucune base de données ou back‑end n’est nécessaire pour des iframes.
- Si un jeu ne se charge pas, vérifiez la console du navigateur : il se peut que la source interdise l’affichage en iframe.
- Pour un domaine personnalisé, ajoutez un fichier `CNAME` à la racine du dépôt contenant votre domaine.

Bon jeu !
