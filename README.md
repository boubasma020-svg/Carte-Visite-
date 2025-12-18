# Carte de Visite Professionnelle

Une carte de visite numérique élégante et interactive avec sauvegarde automatique des données.

## 🌟 Fonctionnalités

### ✨ Design
- **Interface élégante** en noir et blanc avec effets de survol
- **Responsive** - S'adapte automatiquement à tous les appareils (mobile, tablette, desktop)
- **Animations fluides** pour une meilleure expérience utilisateur

### 🔒 Sécurité
- **Protection par mot de passe** pour l'édition
- Seuls les administrateurs peuvent modifier les informations
- Les visiteurs peuvent uniquement télécharger le contact

### 💾 Sauvegarde Automatique
- **LocalStorage** - Toutes les modifications sont sauvegardées automatiquement
- Les données persistent entre les sessions de navigation
- Chargement automatique au démarrage

### 📱 Fonctionnalités Interactives
- **Upload de photo** - Ajoutez votre photo de profil
- **Édition en ligne** - Modifiez toutes les informations directement
- **Export vCard** - Téléchargez le contact au format .vcf

## 🚀 Utilisation

### Pour les Visiteurs
1. Consultez les informations de contact
2. Cliquez sur "Ajouter aux Contacts" pour télécharger la vCard
3. Importez la vCard dans votre application de contacts

### Pour l'Administrateur
1. Cliquez sur le bouton "✏️ Modifier"
2. Entrez le mot de passe administrateur (par défaut: `admin123`)
3. Modifiez les informations:
   - Nom et prénom
   - Titre professionnel
   - Email
   - Téléphone
   - Adresse
   - Photo de profil (cliquez sur la photo)
4. Cliquez sur "✓ Terminé" pour sauvegarder

**Les données sont automatiquement sauvegardées dans le navigateur !**

## 🔧 Configuration

### Changer le Mot de Passe

Ouvrez le fichier `business-card.html` dans un éditeur de texte et trouvez la ligne:

```javascript
const ADMIN_PASSWORD = 'admin123';
```

Remplacez `'admin123'` par votre propre mot de passe sécurisé.

## 📱 Responsive Design

La carte s'adapte automatiquement:

- **Desktop** (> 768px): Design horizontal avec photo à gauche
- **Tablette** (480px - 768px): Design vertical centré
- **Mobile** (< 480px): Design compact optimisé

## 💾 Stockage des Données

### LocalStorage (Actuel)
- Stockage dans le navigateur local
- Données persistantes même après fermeture du navigateur
- Fonctionne sans serveur backend
- **Limitation**: Les données sont spécifiques au navigateur et appareil

### Pour un Stockage Backend (Optionnel)
Si vous souhaitez synchroniser les données sur plusieurs appareils, vous pouvez:
1. Créer une API backend (Node.js, PHP, Python, etc.)
2. Utiliser une base de données (MySQL, MongoDB, Firebase, etc.)
3. Modifier les fonctions `saveData()` et `loadSavedData()` pour utiliser des requêtes HTTP

## 🌐 Déploiement

### GitHub Pages
1. Allez dans **Settings** de votre dépôt
2. Section **Pages** dans la barre latérale
3. Source: **Deploy from a branch**
4. Branche: **master** / Dossier: **/ (root)**
5. Cliquez sur **Save**

Votre carte sera accessible à:
```
https://boubasma020-svg.github.io/Carte-Visite-/business-card.html
```

## 📋 Technologies Utilisées

- **HTML5** - Structure
- **CSS3** - Styles et animations
  - Flexbox pour la mise en page
  - Media queries pour le responsive
  - Gradients et transitions
- **JavaScript Vanilla** - Interactivité
  - LocalStorage API pour la persistance
  - FileReader API pour l'upload d'images
  - Blob API pour l'export vCard

## 📞 Support

Pour toute question ou problème:
- Ouvrez une issue sur GitHub
- Contactez l'administrateur du projet

## 📄 Licence

Ce projet est libre d'utilisation et de modification.

---

🤖 Généré avec [Claude Code](https://claude.com/claude-code)
