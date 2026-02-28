# 🦓 Éditions du Zébrycorne — Site Vitrine

## 📁 Structure des fichiers

```
zebrycorne-site/
├── index.html          ← Page principale
├── style.css           ← Feuille de style
├── script.js           ← Scripts
├── bandeau.jpg         ← Votre bannière (à placer ici)
├── ZebryCorne_net.png  ← Votre logo sans cercle (à placer ici)
└── README.md           ← Ce fichier
```

## 🚀 Mise en ligne sur GitHub Pages — Procédure complète

### ÉTAPE 1 — Créer le dépôt GitHub
1. Allez sur **github.com** et connectez-vous
2. Cliquez sur le bouton vert **"New"** (ou le **+** en haut à droite → New repository)
3. Nommez le dépôt exactement : `zebrycorne-editions` (ou votre préférence)
4. Cochez **"Public"**
5. Cliquez **"Create repository"**

### ÉTAPE 2 — Uploader les fichiers
1. Sur la page du dépôt, cliquez **"uploading an existing file"** (ou Add file → Upload files)
2. Glissez-déposez TOUS les fichiers du dossier :
   - index.html
   - style.css
   - script.js
   - bandeau.jpg
   - ZebryCorne_net.png
3. En bas, écrivez un message : "Premier dépôt du site"
4. Cliquez **"Commit changes"**

### ÉTAPE 3 — Activer GitHub Pages
1. Allez dans **Settings** (onglet en haut du dépôt)
2. Dans le menu gauche, cliquez **"Pages"**
3. Sous "Branch", sélectionnez **"main"** puis **"/ (root)"**
4. Cliquez **"Save"**
5. Attendez 2-3 minutes ☕

### ÉTAPE 4 — Votre site est en ligne !
Votre adresse sera : `https://VOTRE-PSEUDO.github.io/zebrycorne-editions`

---

## ✏️ Personnaliser le site

### Ajouter un livre au catalogue
Dans `index.html`, trouvez la section `<!-- CATALOGUE -->` et copiez-collez un bloc `book-card` :
```html
<div class="book-card">
  <img src="ma-couverture.jpg" alt="Titre" class="book-cover" />
  <div class="book-info">
    <span class="book-genre">Héroïc Fantasy</span>
    <h4>Titre du roman</h4>
    <p class="book-author">Prénom Nom</p>
    <p class="book-desc">Description du livre...</p>
    <a href="#" class="btn-book">En savoir plus</a>
  </div>
</div>
```

### Ajouter un auteur
Dans la section `<!-- AUTEURS -->`, copiez un bloc `author-card` et remplacez les infos.

### Changer l'email de contact
Cherchez `contact@zebrycorne-editions.fr` dans `index.html` et remplacez par votre vrai email.

### Activer le formulaire de contact (envoi réel)
1. Créez un compte gratuit sur **formspree.io**
2. Créez un formulaire et copiez votre ID (ex: `xpzgdabc`)
3. Dans `script.js`, remplacez la simulation par :
```javascript
fetch('https://formspree.io/f/VOTRE-ID', {
  method: 'POST',
  body: new FormData(form),
  headers: { 'Accept': 'application/json' }
})
```

### Domaine personnalisé (optionnel ~10€/an)
1. Achetez un domaine sur **OVH** ou **Gandi** (ex: zebrycorne-editions.fr)
2. Dans GitHub Pages → Custom domain, entrez votre domaine
3. Chez votre registrar, ajoutez les DNS GitHub indiqués dans la doc

---

## 📱 Réseaux sociaux
Dans `index.html`, cherchez les liens Facebook/Instagram et remplacez `href="#"` par vos vraies URLs.
