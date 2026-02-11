Faille de secu owasp

##A01:2021 – Broken Access Control (Contrôle d’accès défaillant)
###Position dans le OWASP Top 10 : #1 (anciennement #5 en 2017)

Le contrôle d’accès défaillant est devenu la vulnérabilité la plus critique du OWASP Top 10 2021. <br> Cette faille permet à un attaquant d’accéder à des ressources, données ou fonctionnalités pour lesquelles il n’a pas d’autorisation.

###Exemples d’attaques :
- Modification d’URL pour accéder à des pages administrateur (/admin)
- Manipulation d’identifiants dans les requêtes (user_id=123 → user_id=456)
- Élévation de privilèges via des tokens mal sécurisés
- Accès direct aux objets (IDOR – Insecure Direct Object Reference)

###Solutions de protection :
- Implémenter des contrôles d’accès côté serveur (jamais uniquement côté client)
- Adopter le principe du moindre privilège (least privilege)
- Refuser l’accès par défaut (deny by default)
- Journaliser tous les échecs de contrôle d’accès
- Effectuer des tests de sécurité réguliers sur les permissions
