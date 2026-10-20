# So Info Gestion — première version déployable

Application web responsive/PWA pour So Info — Réparation & Maintenance. Interface en français, identité noire et jaune et logo fourni intégré.

## Déploiement GitHub Pages
1. Créez un dépôt GitHub (par exemple `so-info-gestion`).
2. Téléversez **tout le contenu** de ce dossier à la racine du dépôt (index.html, app.js, styles.css, manifest, sw.js, logo et dossier icons).
3. Dans **Settings → Pages**, sélectionnez `Deploy from a branch`, branche `main`, dossier `/ (root)`, puis enregistrez.
4. Ouvrez l'URL GitHub Pages affichée par GitHub en HTTPS.
5. Sur iPhone, ouvrez cette URL dans Safari, touchez **Partager → Sur l’écran d’accueil**.

## Fonctions incluses
- Répertoire clients, recherche, tri, modification, confirmation de suppression et historique des documents.
- Création et édition de devis, factures et fiches de prise en charge.
- Calculs par ligne (quantité, prix HT, taux de TVA) et remise globale.
- Conversion d'un devis en brouillon de facture.
- Suivi de statut des factures et paiements.
- Fiche matériel, deux signatures tactiles, aperçu et impression via la boîte de dialogue du navigateur.
- Réglages d'entreprise, sauvegarde JSON, restauration contrôlée et export du journal technique.
- Manifeste PWA, icônes, cache statique versionné et interface mobile avec zones de sécurité iOS.

## Limites importantes à traiter avant usage professionnel
- **Stockage local uniquement** : données dans le stockage du navigateur de cet appareil. Effacer les données du site ou changer de navigateur peut les perdre. Exportez des sauvegardes régulièrement. Pas d'authentification ni de synchronisation multi-appareils.
- Les signatures et données clients sont stockées dans le navigateur local sans chiffrement applicatif. Ne stockez pas de codes de déverrouillage ou mots de passe.
- Le bouton d'impression ouvre une page d'impression; choisissez « Enregistrer au format PDF » dans le navigateur. Le partage natif est limité et ne joint pas encore un vrai PDF.
- Aucun envoi d'e-mail réel n'est implémenté. L'adresse configurée sert de paramètre d'entreprise.
- La numérotation est locale à ce navigateur et ne peut garantir l'unicité si plusieurs appareils sont utilisés. La numérotation et la conservation réglementaire doivent être validées avant production.
- Une facture émise est protégée contre la modification dans cette interface, mais le flux d'avoirs/corrections réglementaires n'est pas encore implémenté.
- Le calcul TVA de cette première version applique le taux de chaque ligne puis prorate la remise globale; validez ce traitement avec votre comptable. La mention de franchise en base doit être vérifiée et configurée selon votre situation réelle.
- La restauration remplace les données existantes après confirmation. Gardez plusieurs sauvegardes hors appareil.
- La génération PDF, la PWA et les signatures n'ont pas été testées sur un iPhone physique ni sur tous les navigateurs. Le journal signale des événements observés, pas une certification que « tout fonctionne ».

## Vérifications recommandées avant utilisation réelle
1. Déployer dans un dépôt privé/public selon votre choix et HTTPS.
2. Tester création client → devis → conversion facture → impression PDF.
3. Tester fiche de prise en charge et signatures sur iPhone Safari.
4. Exporter une sauvegarde, créer des données de test, restaurer et vérifier les enregistrements.
5. Vérifier les mentions légales, TVA, numérotation et obligations de conservation avec un professionnel compétent.
6. Ne pas utiliser de données clients réelles avant d'avoir validé ces parcours.

## Données
Aucune donnée de démonstration n'est préchargée. Les seuls paramètres initiaux sont le nom commercial et l'adresse de réponse fournie dans le cahier des charges.
