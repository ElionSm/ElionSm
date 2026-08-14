<picture>
  <source media="(prefers-color-scheme: dark)" srcset="banner-dark.svg">
  <img alt="Samuel Boisneault — sécurité applicative, DevSecOps" src="banner-light.svg" width="100%">
</picture>

<br>

Je construis des backends, puis je cherche par où ils cèdent.

Étudiant ingénieur en cybersécurité à **ESIEE Paris** (5ᵉ année, cursus labellisé
SecNumedu par l'ANSSI). Je cherche un **stage de fin d'études de 6 mois à partir de
février 2027**, en sécurité applicative, DevSecOps ou sécurité cloud.

<br>

## Projets

### [agent-memory-security](https://github.com/ElionSm/agent-memory-security)

Une mémoire persistante d'agent LLM peut être empoisonnée par un simple fichier local :
l'instruction devient un souvenir, le souvenir survit à la session, et il ressort plus tard
pour justifier un appel d'outil. Ce dépôt reproduit cette baseline vulnérable, puis construit
autour d'elle une autorité de mémoire liée à l'origine — une mémoire ne peut justifier une
action que si sa provenance lui en donne le droit.

Toute la chaîne `source → mémoire → rappel → tâche → appel d'outil` est persistée et
auditable, et chaque rejet porte un code stable. Les destinations sensibles sont
systématiquement simulées : rien n'est jamais envoyé.

`Python 3.12` · `SQLite` · `Ollama` · `pytest` · `ruff` · `mypy`

### [websec-labs](https://github.com/ElionSm/websec-labs)

Mes notes sur les labs de la Web Security Academy de PortSwigger — injection SQL, contrôle
d'accès, SSRF, désérialisation. Une règle : aucune assistance tant que le lab n'est pas
résolu. L'objectif est de reconnaître une construction vulnérable à vue, et déléguer cette
étape ne produit rien.

`Markdown` · en cours

### [photo-sorter-windows](https://github.com/ElionSm/photo-sorter-windows)

Application de bureau pour trier les photos d'un téléphone et les exporter vers une archive.
Import incrémental, déduplication par empreinte SHA-256, file de traitement asynchrone et
cache LRU de vignettes. Petit outil, mais fini et réellement utilisé.

`C#` · `WinUI` · `SQLite`

<br>

## Expérience

**Orange** — stagiaire ingénieur, sécurité applicative et automatisation de tests
· mai à août 2026 · équipe backend Java.

Une plateforme interne d'automatisation des campagnes de tests de non-régression, un service
Go de collecte de traces OpenTelemetry, et le volet sécurité de l'ensemble : modèle de menaces
STRIDE, protection des secrets, validation stricte des certificats TLS, purges en simulation
par défaut, et vérification d'intégrité des binaires tiers qui casse le build en cas d'écart.

C'est de là que vient la seule règle que je garde de ce stage : **un contrôle qui ne produit
pas de décision n'a rien produit.** Une empreinte qu'on se contente de journaliser n'est pas
un contrôle ; une empreinte qui arrête la construction en est un.

<br>

## Outils

**Langages** — Java 17, Go, Python, C#, SQL, Bash
**Plateforme** — Spring Boot, GitLab CI/CD, Docker, AWS, Cloud Foundry, MongoDB, OpenTelemetry
**Sécurité** — OWASP Top 10 et ASVS, STRIDE, CWE, ISO/IEC 27001

<br>

## Me joindre

[LinkedIn](https://www.linkedin.com/in/samuel-boisneault) · samuelboisneault.pro@gmail.com
