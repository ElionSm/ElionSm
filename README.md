<a href="https://elionsm.github.io/">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="banner-dark.svg">
    <img alt="Samuel Boisneault, étudiant ingénieur en cybersécurité à l'ESIEE Paris" src="banner-light.svg" width="100%">
  </picture>
</a>

<br>

Je construis des backends, puis je cherche par où ils cèdent.

Étudiant ingénieur en cybersécurité à **ESIEE Paris** (5ᵉ année, cursus labellisé
SecNumedu par l'ANSSI). Je cherche un **stage de fin d'études de 6 mois à partir de
février 2027**, en sécurité applicative, DevSecOps, sécurité cloud ou sécurité des
agents IA.

**[Lire mon CV](https://elionsm.github.io/)** en français ou en anglais, ou
[m'écrire](mailto:samuelboisneault.pro@gmail.com).

<br>

## Projets

### [agent-memory-security](https://github.com/ElionSm/agent-memory-security)

Une mémoire persistante d'agent LLM peut être empoisonnée par un simple fichier local :
l'instruction devient un souvenir, le souvenir survit à la session, et il ressort plus tard
pour justifier un appel d'outil. Ce dépôt reproduit cette baseline vulnérable, puis construit
autour d'elle une autorité de mémoire liée à l'origine : une mémoire ne peut justifier une
action que si sa provenance lui en donne le droit.

Toute la chaîne `source → mémoire → rappel → tâche → appel d'outil` est persistée et
auditable, et chaque rejet porte un code stable. Les destinations sensibles sont
systématiquement simulées : rien n'est jamais envoyé.

`Python 3.12` `SQLite` `Ollama` `pytest` `ruff` `mypy`

### [photo-sorter-windows](https://github.com/ElionSm/photo-sorter-windows)

Application de bureau pour trier les photos d'un téléphone et les exporter vers une archive.
Import incrémental, déduplication par empreinte SHA-256, file de traitement asynchrone et
cache LRU de vignettes. Petit outil, mais fini et réellement utilisé.

`C#` `WinUI` `SQLite`

### Projets d'école

**Infrastructure CI/CD sécurisée sur AWS** (ESIEE, 2026, équipe de quatre). Pipeline
Jenkins, SonarQube, Maven et Nexus sur EC2, derrière Nginx, avec un accès d'administration
réservé au VPN WireGuard. Ma part : la chaîne Jenkins, et Fail2Ban sur les logs Nginx, avec
un filtre écrit à la main contre les scans de pages, un bannissement immédiat au premier
dépassement de débit et une jail de récidive.

**NeXusGate** (ESIEE, 2025). Portique de contrôle d'accès par reconnaissance faciale 3D,
dont j'ai mené la partie réseau ; données biométriques traitées selon l'article 9 du RGPD.
Prix du meilleur projet technique de l'ESIEE 2025, parmi plus de 75 projets.

<br>

## Expérience

**Orange**, stagiaire ingénieur en sécurité applicative, automatisation de tests et CI/CD.
Mai à août 2026, équipe backend Java, Arcueil.

J'y ai conçu une plateforme interne d'automatisation des tests de non-régression, branchée
sur les pipelines GitLab CI/CD et sécurisée par OAuth 2.0 : une dizaine de campagnes de
plusieurs centaines de tests tournent chaque jour. Autour d'elle, une analyse de couverture
hybride (JavaParser, JaCoCo, OpenTelemetry) et un service Go de collecte des traces. En
instrumentant une application interne, j'ai trouvé une vulnérabilité, puis mené l'analyse
d'impact et le correctif.

De ma propre initiative, j'ai pris en charge le volet sécurité de la plateforme : modèle de
menaces STRIDE, protection des secrets, validation stricte des certificats TLS, purges en
simulation par défaut, et vérification d'intégrité des binaires tiers qui casse le build en
cas d'écart.

C'est de là que vient la seule règle que je garde de ce stage : **un contrôle qui ne produit
pas de décision n'a rien produit.** Une empreinte qu'on se contente de journaliser n'est pas
un contrôle ; une empreinte qui arrête la construction en est un.

<br>

## En ce moment

Les labs de la Web Security Academy de PortSwigger, avec une règle : aucune aide tant que le
lab n'est pas résolu. L'objectif est de reconnaître une construction vulnérable à vue, et
déléguer cette étape ne produit rien.

<br>

## Outils

- **Sécurité** : OWASP Top 10, OWASP Top 10 pour les LLM, ASVS, STRIDE, CWE / CAPEC, OAuth 2.0, Burp Suite, notions d'ISO/IEC 27001
- **DevSecOps** : GitLab CI/CD, Jenkins, SonarQube, Nexus, Docker, Fail2Ban, WireGuard
- **Langages** : Java 17, Python, Go, C#, SQL, Bash
- **Plateforme** : Spring Boot, AWS, Cloud Foundry, MongoDB, OpenTelemetry

<br>

## Me joindre

[CV](https://elionsm.github.io/) · [LinkedIn](https://www.linkedin.com/in/samuel-boisneault) · [samuelboisneault.pro@gmail.com](mailto:samuelboisneault.pro@gmail.com)
