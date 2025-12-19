📌 Capture The Flag

🎯 Objectif du projet :
Ce projet s’inscrit dans le cadre d’un Capture The Flag (CTF) orienté sécurité applicative.
L’objectif est d’identifier, exploiter, documenter puis corriger plusieurs vulnérabilités de sécurité présentes dans une application web volontairement vulnérable.
L’approche retenue est à la fois offensive (détection/exploitation) et défensive (remédiation), conformément aux bonnes pratiques de la cybersécurité moderne.
======================================================================================================================================================================
🔍 Vulnérabilités à identifier :
Les failles suivantes doivent être trouvées et documentées :
- 2 vulnérabilités de type XSS (Cross-Site Scripting)
- 2 vulnérabilités de type Injection SQL
- BONUS : découverte de flags supplémentaires liés à d’autres failles de sécurité

Chaque vulnérabilité fait l’objet :
- d’une description technique,
- d’une preuve d’exploitation (payload, requête, screenshots dans le répertoire portant le nom de la vulnérabilité),
======================================================================================================================================================================
🛠️ Phase de remédiation :
À l’issue de l’exploitation, un correctif est proposé et implémenté pour chaque vulnérabilité identifiée.

Les correctifs visent à :
- éliminer la cause racine de la faille,
- renforcer la validation et le traitement des entrées utilisateur,
- réduire la surface d’attaque globale de l’application.
======================================================================================================================================================================
🔐 Bonnes pratiques :
Les correctifs appliqués respectent les principes du OWASP Top 10, notamment :
- Validation stricte des entrées utilisateur
- Encodage et échappement des sorties
- Utilisation de requêtes préparées contre les injections SQL
- Principe du moindre privilège

Règle d’or de la sécurité applicative “Never trust user input”

⚠️ Avertissement
Ce projet est réalisé exclusivement à des fins pédagogiques.
Toute exploitation de vulnérabilités en dehors d’un cadre légal et autorisé est strictement interdite.
