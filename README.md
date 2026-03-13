## 🏴‍☠️ Capture The Flag – Born2Sec

![OWASP](https://img.shields.io/badge/OWASP-Top%2010-000000?logo=owasp&logoColor=white)
![CTF](https://img.shields.io/badge/Capture%20The%20Flag-Active-purple?logo=flag&logoColor=white)
![Security](https://img.shields.io/badge/Security-Hardening-blue?logo=shield&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-Hardened-black?logo=linux&logoColor=white)

## Ce CTF a pour objectif d’explorer et d’exploiter différentes vulnérabilités issues du top OWASP, dans un environnement contrôlé. Chaque étape permet de comprendre une faille, de l’exploiter, puis d’appliquer une mesure corrective.

---

## 🎯 Objectifs du projet :

- Identifier des vulnérabilités web courantes
- Exploiter des failles de manière contrôlée
- Comprendre l’impact réel d’une mauvaise configuration
- Apprendre à corriger et sécuriser un service web
- Développer une démarche offensive → défensive

---

## 🧩 Structure du CTF (chaque challenge correspondant à une vulnérabilité OWASP)

## 🔹 Challenge 1 — Injection SQL
Objectif : contourner l’authentification

```
Exploit : ' OR 1=1 --
```

```
Flag : FLAG{SQLI_SUCCESS}
```

=> Fix : requêtes préparées + validation stricte

## 🔹 Challenge 2 — XSS (Cross‑Site Scripting)
Objectif : exécuter du JavaScript dans le navigateur

```
Exploit : <script>alert(1)</script>
```

```
Flag : FLAG{XSS_PWNED}
```

=> Fix : escaping + CSP

## 🔹 Challenge 3 — Directory Traversal
Objectif : lire un fichier sensible

```
Exploit : ../../../../etc/passwd
```

```
Flag : FLAG{TRAVERSAL_OK}
```

=> Fix : whitelist + path normalisation

## 🔹 Challenge 4 — Mauvaise configuration serveur
Objectif : accéder à une page admin exposée

```
Exploit : /admin/
```

```
Flag : FLAG{MISCONFIG_FOUND}
```

=> Fix : durcissement + permissions

## 🔹 Challenge 5 — Faiblesse d’authentification
Objectif : brute‑forcer un mot de passe faible

```
Exploit : admin:admin
```

```
Flag : FLAG{AUTH_BROKEN}
```

=> Fix : MFA + politique de mot de passe

---

## 🏆 Validation des flags
Chaque challenge valide un flag sous forme :

```
FLAG{NOM_DU_CHALLENGE}
```

---

## 🔐 Partie Défensive (Hardening)
Après exploitation, il faut concevoir une section “Fix & Hardening” :

- patch serveur
- configuration sécurisée
- headers HTTP
- permissions
- logs
- monitoring
- tests automatisés
