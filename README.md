# Laboratoire International de Chimie Monétaire - Site Vitrine

Site web vitrine professionnel créé selon le cahier des charges fourni.

## Structure du site

### Pages principales
- **index.html** - Page d'accueil avec hero, présentation, services et contact rapide
- **presentation.html** - Présentation de l'entreprise avec mission et valeurs
- **multimedia.html** - Galerie photos
- **devis.html** - Formulaire de demande de devis
- **contact.html** - Page de contact avec formulaire et coordonnées
- **mentions-legales.html** - Mentions légales
- **sitemap.html** - Plan du site

### Pages de prestations (dossier services/)
- **nettoyage.html** - Service de nettoyage de billets
- **impression.html** - Service d'impression de billets
- **materiels.html** - Matériels et produits
- **consulting.html** - Consulting et conseils

## Fonctionnalités

✅ Navigation responsive avec Bootstrap 5
✅ Design institutionnel moderne
✅ Animations CSS (fadeIn, slideIn, hover effects)
✅ Cartes services avec numéros (01, 02, 03, 04)
✅ Bouton WhatsApp flottant avec message pré-rempli
✅ Formulaire de demande de devis avec validation
✅ Formulaire de contact
✅ Coordonnées complètes (adresse, 2 e-mails, téléphone, WhatsApp)
✅ Footer avec mentions légales et sitemap
✅ SEO optimisé (meta tags, titles, descriptions)
✅ Responsive (mobile, tablette, desktop)

## Images

Les images du dossier `images/` sont utilisées dans tout le site :
- hero-new.jpg - Image hero (background)
- laboratoire.jpg - Présentation du laboratoire
- team.jpg - Photo de l'équipe
- nettoyage-new.jpg - Service nettoyage
- slide1.jpg - Service impression / Carousel 1
- slide2.jpg - Service matériels / Carousel 2
- slide3.jpg - Service consulting / Carousel 3
- slide4.jpg - Carousel 4
- equipment1.jpg - Équipements multimédia
- equipment2.jpg - Équipements multimédia
- gallery1-4.jpg - Galerie multimédia supplémentaire

## Comment visualiser le site

### Option 1: Ouvrir directement
Ouvrez simplement le fichier `index.html` dans votre navigateur.

### Option 2: Serveur local
Si vous avez Python installé :
```bash
cd C:\Users\DENIS FBI-STORE\Desktop\site
python -m http.server 8000
```
Puis ouvrez http://localhost:8000 dans votre navigateur.

### Option 3: Serveur PHP
Si vous avez PHP installé :
```bash
cd C:\Users\DENIS FBI-STORE\Desktop\site
php -S localhost:8000
```

## Personnalisation

### Modifier les couleurs
Dans `styles.css`, modifiez les variables CSS en haut du fichier :
```css
:root {
    --primary-color: #0d6efd;
    --secondary-color: #6c757d;
    --accent-color: #ffc107;
    --dark-color: #212529;
    --light-color: #f8f9fa;
}
```

### Modifier les coordonnées
Les coordonnées sont dans chaque page HTML. Modifiez-les dans :
- La section "Contact rapide" de index.html
- La section "Coordonnées" de presentation.html
- La page contact.html

### Formulaire backend
Les formulaires sont actuellement en mode statique (JavaScript valide les données). Pour rendre les formulaires fonctionnels avec envoi réel, vous devez :
1. Ajouter un backend (PHP, Node.js, etc.)
2. Configurer un serveur de messagerie
3. Modifier les fonctions JavaScript `handleQuoteForm` et `handleContactForm` pour envoyer les données au serveur

## Remarques sur les vidéos

Le site original (labochimiemonetaire.com) n'a pas de vidéos sur sa page multimédia. Par conséquent, cette version n'inclut pas de section vidéo, conformément au site original.

## Technologies utilisées

- **HTML5** - Structure sémantique
- **CSS3** - Styles et animations
- **Bootstrap 5.3.2** - Framework CSS responsive
- **Font Awesome 6.5.1** - Icônes
- **JavaScript (ES6+)** - Interactions et validation

## Sécurité

Pour une mise en production, assurez-vous de :
1. Activer HTTPS/SSL
2. Valider et sécuriser les formulaires côté serveur
3. Protéger contre les attaques XSS et CSRF
4. Utiliser des mots de passe forts pour l'administration (si implémentée)
5. Mettre en place des sauvegardes automatiques

## Support

Pour toute question ou modification nécessaire, contactez l'équipe de développement.