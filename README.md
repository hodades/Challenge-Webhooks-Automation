# Webhook Automation
# README - Challenge Webhooks

Ce projet est une solution pour le défi "Challenge Webhooks", qui consiste à communiquer entre plusieurs webhooks et implémenter une logique de vérification avec une base de données.

## Fonctionnalités

- **Communication entre Webhooks** : Connecte deux ou plusieurs webhooks pour permettre l'échange de données avec une étape de recherche.
- **Gestion des utilisateurs** : En fonction de la présence ou non de l'email dans la base de données, différentes actions sont effectuées.
- **Envoi de mails automatisé** : Si l'email est absent de la base de données, un mail d'inscription est envoyé.

## Bonnes Pratiques

- **Nommer les webhooks** : Pour une meilleure organisation, il est recommandé de donner des noms clairs aux webhooks.
- **Activer les webhooks** : Vérifiez toujours que le webhook est activé avant d'envoyer les données.
- **Éviter les modifications simultanées** : Travaillez sur un webhook à la fois pour éviter les erreurs liées aux scénarios en mode édition.
- **Utilisation du JavaScript** : Attention à la manipulation du JavaScript dans les réponses à des requêtes.

## Utilisation

1. **Paramètre d'URL** : Lorsque vous envoyez une requête à votre webhook, vous pouvez passer l'email de la personne comme paramètre dans l'URL.
2. **Réponse personnalisée** : Si l'email est présent dans la base de données, une réponse personnalisée sera affichée avec les informations telles que le prénom, la profession, et l'emplacement géographique.

### Exemple de réponse
- **Email trouvé** :
  ```
  Welcome back {{Prénom}},
  Quel temps fait-il à {{Emplacement géographique}} ? Toujours {{Profession}} ?
  ```

- **Email non trouvé** :
  ```
  Bienvenue, veuillez vérifier votre boîte mail pour finaliser votre inscription.
  ```

Un lien vers un formulaire sera envoyé pour permettre à l'utilisateur de s'enregistrer.

## Liens utiles

- [Google Spreadsheet](https://docs.google.com/spreadsheets/d/1G_NZIksi-3KcxidLEvAuMNc-n7i6rr8oddPb0FO7RhE/edit?gid=0#gid=0) : Suivi des utilisateurs et des réponses.

## Licence

Ce projet est sous licence MIT.


