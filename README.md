# BlogSphere - Plateforme de Blog Moderne

## 📁 Structure du Projet

```
Frontend/
├── backend/                 # Backend PHP
│   ├── api/                # API endpoints
│   │   ├
│   │   ├── inscription.php # Page d'inscription
│   │   ├── check_session.php # Vérification de session
│   │   ├── create_article.php # Création d'articles
│   │   ├── save_article.php # Sauvegarde d'articles
│   │   └── upload_cover.php # Upload d'images
│   ├── classes/            # Classes PHP
│   │   ├── database.php    # Gestion de la BDD
│   │   └── user.php        # Gestion des utilisateurs
│   ├── config/             # Configuration
│   │   ├── config.php      # Configuration centrale
│   │   └── db_schema.sql   # Schéma de la base de données
│   ├── uploads/            # Fichiers uploadés
│   │   ├── covers/         # Images de couverture
│   │   └── avatars/        # Avatars utilisateurs
│   └── .htaccess           # Sécurité du backend
├── css/                    # Styles CSS
├── js/                     # JavaScript
├── assets/                 # Ressources statiques
├── accueil.html           # Page d'accueil
├── articles.html          # Liste des articles
├── article.html           # Affichage d'un article
├── inscription.php       # Page d'inscription
├── connexion.php         # Page de connexion
├── edition-article.php    # Éditeur d'articles
└── userprofile.html       # Profil utilisateur
```

## 🚀 Fonctionnalités

### **Backend (PHP)**
- ✅ **API RESTful** pour la gestion des articles
- ✅ **Système d'authentification** sécurisé
- ✅ **Upload d'images** avec validation
- ✅ **Base de données** MySQL avec PDO
- ✅ **Configuration centralisée** et sécurisée
- ✅ **Gestion des sessions** et sécurité CSRF

### **Frontend (HTML/CSS/JS)**
- ✅ **Éditeur WYSIWYG** avec support Markdown
- ✅ **Coloration syntaxique** pour les blocs de code
- ✅ **Interface responsive** et moderne
- ✅ **Gestion des brouillons** et publication
- ✅ **Upload d'images** de couverture
- ✅ **Raccourcis clavier** pour l'édition

## 🛠️ Installation

1. **Cloner le projet**
   ```bash
   git clone [url]
   cd Frontend
   ```

2. **Configurer la base de données**
   ```bash
   # Importer le schéma
   mysql -u root -p < backend/config/db_schema.sql
   ```

3. **Configurer l'application**
   - Modifier `backend/config/config.php` selon votre environnement
   - Ajuster les URLs dans la configuration

4. **Démarrer le serveur**
   ```bash
   php -S localhost:8000
   ```

## 🔧 Configuration

### **Base de données**
- Host: `localhost`
- Database: `blogsphere`
- User: `root`
- Password: `[votre-mot-de-passe]`

### **Uploads**
- Taille max: 5MB
- Types autorisés: JPG, PNG, GIF, WebP
- Dossiers: `backend/uploads/covers/` et `backend/uploads/avatars/`

## 📝 Utilisation

1. **Inscription/Connexion** : `inscription.php` ou `connexion.php`
2. **Éditer un article** : `edition-article.php`
3. **Voir les articles** : `articles.php`
4. **Page d'accueil** : `accueil.php`

## 🔒 Sécurité

- ✅ **Validation des données** côté serveur
- ✅ **Protection CSRF** sur tous les formulaires
- ✅ **Hachage sécurisé** des mots de passe
- ✅ **Validation des fichiers** uploadés
- ✅ **Sessions sécurisées** avec timeout
- ✅ **Accès restreint** au dossier backend

## 🎯 API Endpoints

- `POST /backend/api/create_article.php` - Créer un article
- `POST /backend/api/save_article.php` - Sauvegarder un article
- `POST /backend/api/upload_cover.php` - Upload d'image
- `GET /backend/api/check_session.php` - Vérifier la session

## 📚 Technologies

- **Backend** : PHP 8+, MySQL, PDO
- **Frontend** : HTML5, CSS3, JavaScript ES6+
- **Éditeur** : Markdown, WYSIWYG, Highlight.js
- **Sécurité** : Sessions PHP, CSRF, Validation
