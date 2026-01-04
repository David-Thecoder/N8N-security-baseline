## RègLe de sécurité(N8)
Le service SSH doit etre configure de maniere stricte :
1. Pas d'authentification par mot de passe.
2. Pas de connexion root.

## Logique d'Automatisation(n8n)
1. Trigger: Toutes les 6h.
2. Action: Verifier la config SSH du serveur cible.
3.Condition: Si 'PasswordAuth==yes' ALORS Alerte.
4.Alerte: Notification Slack immédiate.
