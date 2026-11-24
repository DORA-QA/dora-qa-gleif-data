# DORA QA — copie GLEIF

Copie des données publiques du **GLEIF** (Golden Copy : LEI et relations), mise en forme en Parquet pour la **version en ligne** de [DORA QA](https://github.com/DORA-QA/dora-register-quality-analyst) (DORA Register Quality Analyst).

- Mise à jour **chaque nuit** par le workflow *GLEIF copy* (02:30 UTC), avec les outils de DORA QA (`backend/tools/build_gleif.py`).
- Publiée en releases `gleif-AAAAMMJJ-HHMM` : `manifest.json` (date de publication GLEIF, SHA-256 de chaque fichier), `lei.parquet`, `rr.parquet`.
- **Seules les 2 dernières copies (2 jours) sont gardées.**
- La version en ligne de DORA QA télécharge la plus récente au démarrage, sans jeton, avant d'accepter le moindre registre.

## Source et licence des données

Source : **Global Legal Entity Identifier Foundation (GLEIF)**, https://www.gleif.org — données publiées sous licence **Creative Commons CC0 1.0**. Ce dépôt ne contient aucune donnée de registre DORA.

---

Public GLEIF data (LEI and relationships, CC0 1.0) reformatted as Parquet for the online version of DORA QA. Rebuilt every night; only the last 2 copies are kept.
