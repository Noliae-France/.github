<div align="center">

# Noliae‑France

### Logiciels souverains, écrits en **Nolc** — un langage compilé, sans dépendance, en français.

Du langage à l'infrastructure : un écosystème cohérent, MIT, testé, sans boîte noire.

<br/>

![Paquets](https://img.shields.io/badge/paquets-39-FF4D2E?style=flat-square)
![Langage](https://img.shields.io/badge/langage-Nolc-111?style=flat-square)
![Licence](https://img.shields.io/badge/licence-MIT-green?style=flat-square)
![CI](https://img.shields.io/badge/CI-verte-2ea44f?style=flat-square)

</div>

---

## 🧩 Le langage Nolc

**Nolc** compile vers du C11 portable puis un binaire natif : pas de machine virtuelle, pas de ramasse‑miettes, mémoire par régions, mots‑clés bilingues (FR/EN). Messages d'erreur en français.

- 📦 **Dernière version du compilateur** : [`nolc-latest-linux-x86_64.tar.gz`](https://noliae-nolc.s3.gra.io.cloud.ovh.net/nolc-latest-linux-x86_64.tar.gz) · [`.deb`](https://noliae-nolc.s3.gra.io.cloud.ovh.net/nolc-latest-amd64.deb) · [`.rpm`](https://noliae-nolc.s3.gra.io.cloud.ovh.net/nolc-latest-x86_64.rpm)
- 🧩 **Extension VS Code** : [`noliae-code-latest.vsix`](https://noliae-nolc.s3.gra.io.cloud.ovh.net/noliae-code-latest.vsix)
- 📚 **Documentation** : [wiki.noliae.com](https://wiki.noliae.com)

```bash
# Installation rapide (Linux x86_64)
curl -fsSL https://noliae-nolc.s3.gra.io.cloud.ovh.net/nolc-latest-linux-x86_64.tar.gz | tar xz
sudo cp nolc-*/nolc /usr/local/bin/
```

---

## 📚 L'écosystème `nol-*`

Des bibliothèques **pures Nolc**, sans dépendance, chacune testée avec CI verte. Ajoutez‑en une à votre projet :

```toml
[dependances]
"nol-cache" = { git = "https://github.com/Noliae-France/nol-cache" }
```

### 🌐 Web

| Paquet | Rôle |
|---|---|
| [**nol-http**](https://github.com/Noliae-France/nol-http) | Briques serveur HTTP : routage, parsing requête, en‑têtes |
| [**nol-serde**](https://github.com/Noliae-France/nol-serde) | Sérialisation JSON correcte (échappement, composition) |
| [**nol-validation**](https://github.com/Noliae-France/nol-validation) | Validation déclarative, erreurs structurées |
| [**nol-auth**](https://github.com/Noliae-France/nol-auth) | Authentification : Bearer, RBAC (sessions/JWT à venir) |
| [**nol-url**](https://github.com/Noliae-France/nol-url) | Analyse d'URL (schéma, hôte, port, chemin, requête) |
| [**nol-cookie**](https://github.com/Noliae-France/nol-cookie) | Cookies : parsing, SameSite, Secure, HttpOnly |
| [**nol-mime**](https://github.com/Noliae-France/nol-mime) | Types MIME par extension de fichier |

### 🗃️ Données & stockage

| Paquet | Rôle |
|---|---|
| [**nol-cache**](https://github.com/Noliae-France/nol-cache) | Cache mémoire TTL/LRU, interface compatible Redis |
| [**nol-sql**](https://github.com/Noliae-France/nol-sql) | Interface SQL commune (pool/pg/sqlite à venir) |
| [**nol-csv**](https://github.com/Noliae-France/nol-csv) | Encodage / décodage CSV (RFC 4180) |

### 🔐 Sécurité & aléa

| Paquet | Rôle |
|---|---|
| [**nol-html**](https://github.com/Noliae-France/nol-html) | Échappement HTML sûr (anti‑XSS) |
| [**nol-uuid**](https://github.com/Noliae-France/nol-uuid) | UUID v4 (aléatoire cryptographique) |
| [**nol-random**](https://github.com/Noliae-France/nol-random) | Aléa crypto : octets, entier borné, hex, choix |

### 🤖 IA & LLM

| Paquet | Rôle |
|---|---|
| [**nol-ai**](https://github.com/Noliae-France/nol-ai) | API IA agnostique du fournisseur (messages, requêtes, JSON) |
| [**nol-llama**](https://github.com/Noliae-France/nol-llama) | Interface vers llama.cpp (modèles GGUF locaux, CPU/GPU) |
| [**nol-prompt**](https://github.com/Noliae-France/nol-prompt) | Templates de prompts typés (variables, versions, cache) |
| [**nol-embedding**](https://github.com/Noliae-France/nol-embedding) | Embeddings : cosinus, normalisation, distances |
| [**nol-vector**](https://github.com/Noliae-France/nol-vector) | Index vectoriel local, recherche des plus proches voisins |

### 💶 Finance & comptabilité

| Paquet | Rôle |
|---|---|
| [**nol-money**](https://github.com/Noliae-France/nol-money) | Montants exacts (unités mineures), devises ISO 4217 |
| [**nol-ledger**](https://github.com/Noliae-France/nol-ledger) | Comptabilité en partie double |
| [**nol-accounting**](https://github.com/Noliae-France/nol-accounting) | Journaux, exercices, clôtures et résultat |
| [**nol-chart**](https://github.com/Noliae-France/nol-chart) | Plans comptables (PCG français) |
| [**nol-invoice**](https://github.com/Noliae-France/nol-invoice) | Devis, factures, avoirs et échéances |
| [**nol-tax**](https://github.com/Noliae-France/nol-tax) | TVA, taxes et règles versionnées |
| [**nol-reconcile**](https://github.com/Noliae-France/nol-reconcile) | Rapprochement bancaire |
| [**nol-payment**](https://github.com/Noliae-France/nol-payment) | Paiements, remboursements, statuts, idempotence |
| [**nol-subscription**](https://github.com/Noliae-France/nol-subscription) | Abonnements et facturation périodique |
| [**nol-treasury**](https://github.com/Noliae-France/nol-treasury) | Trésorerie, positions et prévisions |
| [**nol-assets**](https://github.com/Noliae-France/nol-assets) | Immobilisations et amortissements |
| [**nol-expense**](https://github.com/Noliae-France/nol-expense) | Notes de frais et justificatifs |
| [**nol-payroll-core**](https://github.com/Noliae-France/nol-payroll-core) | Écritures comptables de paie |
| [**nol-audit**](https://github.com/Noliae-France/nol-audit) | Historique immuable (chaîne de hachage) |

### 🛠️ Utilitaires

| Paquet | Rôle |
|---|---|
| [**nol-str**](https://github.com/Noliae-France/nol-str) | Utilitaires de chaînes (pad, tronque, titre, compte…) |
| [**nol-slug**](https://github.com/Noliae-France/nol-slug) | Slugs URL‑friendly (accents FR translittérés) |
| [**nol-path**](https://github.com/Noliae-France/nol-path) | Manipulation de chemins de fichiers |
| [**nol-semver**](https://github.com/Noliae-France/nol-semver) | Versions sémantiques (analyse, comparaison) |
| [**nol-dotenv**](https://github.com/Noliae-France/nol-dotenv) | Chargement de fichiers `.env` |
| [**nol-log**](https://github.com/Noliae-France/nol-log) | Journalisation à niveaux + horodatage |
| [**nol-color**](https://github.com/Noliae-France/nol-color) | Couleurs et styles ANSI pour le terminal |

---

<div align="center">

Fait avec ❤️ en France · Licence **MIT** · Contributions bienvenues

</div>
