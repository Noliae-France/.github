<div align="center">

# Noliae-France

### Des logiciels libres, souverains et respectueux de la vie privée.

**Organisation française à but non lucratif**, Noliae-France développe des outils numériques ouverts au service de nos concitoyennes et concitoyens, particulièrement de celles et ceux qui souhaitent garder le contrôle de leur vie privée.

[Nos projets](https://github.com/orgs/Noliae-France/repositories) · [Nolc](https://github.com/Noliae-France/Nolc) · [NolCore](https://github.com/Noliae-France/NolCore) · [Documentation](https://wiki.noliae.com)

![Logiciels libres](https://img.shields.io/badge/logiciels-libres-FF4D2E?style=flat-square)
![France](https://img.shields.io/badge/conçu_en-France-111111?style=flat-square)
![Vie privée](https://img.shields.io/badge/vie_privée-par_défaut-2ea44f?style=flat-square)

</div>

---

## Notre mission

Nous pensons que les outils numériques essentiels ne devraient pas imposer la surveillance, l’enfermement propriétaire ou l’exploitation des données personnelles. Noliae-France conçoit et publie des logiciels dont le code peut être lu, vérifié, amélioré et réutilisé.

Notre démarche est non lucrative : elle vise l’intérêt général, l’autonomie numérique et l’accès à des services compréhensibles pour toutes et tous.

## Nos engagements

- **Vie privée par défaut** — minimisation des données, protections techniques et choix explicites.
- **Logiciels ouverts** — le code source de nos applications est public afin que chacun puisse l’auditer.
- **Souveraineté et interopérabilité** — des formats ouverts, des déploiements maîtrisables et aucune dépendance inutile à une plateforme.
- **Sécurité concrète** — chiffrement, sessions sécurisées, validation des entrées et intégration continue.
- **Accessibilité** — une expérience lisible, rapide et utile, sans manipulation ni publicité invasive.

## Les projets Noliae

| Projet | Rôle |
|---|---|
| [Nolc](https://github.com/Noliae-France/Nolc) | Langage compilé en C11, conçu pour produire des binaires simples et portables. |
| [NolCore](https://github.com/Noliae-France/NolCore) | Base applicative ouverte : API, utilisateurs, permissions, PostgreSQL, recherche et IA. |
| [Noliae Search](https://github.com/Noliae-France/Noliae-Search) | Interface de recherche reliée au Core. |
| [Noliae IA](https://github.com/Noliae-France/Noliae-IA) | Interface conversationnelle multi-modèles, pilotée par les permissions du Core. |
| [Noliae Account](https://github.com/Noliae-France/Noliae-Account) | Gestion du compte, des sessions et de la sécurité. |

## Nolc et l’écosystème `nol-*`

Nolc compile vers du C11 puis un binaire natif. Le projet privilégie les dépendances réduites, la mémoire par régions, une documentation en français et des outils auditables.

```bash
curl -fsSL https://noliae-nolc.s3.gra.io.cloud.ovh.net/nolc-latest-linux-x86_64.tar.gz | tar xz
sudo cp nolc-*/nolc /usr/local/bin/
```

Retrouvez les bibliothèques web, sécurité, données, recherche et IA dans les [dépôts de l’organisation](https://github.com/orgs/Noliae-France/repositories).

## Participer

Les contributions, retours d’expérience, audits et propositions sont les bienvenus. Avant toute contribution, consultez le README et les documents de sécurité du dépôt concerné.

Si vous utilisez un projet Noliae, signalez les problèmes de manière responsable et évitez de publier des informations sensibles dans une issue publique.

---

<div align="center">

Fait en France, pour des services numériques plus respectueux.
Code ouvert · Contributions bienvenues · Vie privée non négociable

</div>
