# So Info — Assistant de gestion

## Mise en ligne sur GitHub Pages
1. Crée un dépôt GitHub (par exemple `soinfo-gestion`).
2. Décompresse cette archive et envoie `index.html` ainsi que le dossier `assets/` à la racine du dépôt.
3. Dans **Settings → Pages**, choisis **Deploy from a branch**, la branche `main` et le dossier `/ (root)`, puis enregistre.
4. Ouvre l’URL GitHub Pages affichée après publication.

## Fonctionnalités du prototype
- Gestion locale des clients (création, sélection, suppression).
- Fiche de prise en charge, devis et facture.
- Impression / enregistrement en PDF depuis le navigateur.
- Préparation d’un e-mail avec `mailto:` ; il faut joindre le PDF manuellement.
- Export/import JSON pour sauvegarder les clients.

## Limites importantes
- Les données restent dans le navigateur utilisé et ne sont pas synchronisées entre appareils.
- GitHub Pages héberge des fichiers statiques : l’envoi automatique d’e-mails nécessite un backend ou un service tiers sécurisé.
- Les documents sont des modèles de départ. Complète les informations légales et vérifie les règles de facturation applicables à ton entreprise avant de les utiliser.
- Ne stocke pas de mots de passe de clients ni d’informations sensibles.
