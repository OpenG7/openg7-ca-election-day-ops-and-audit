# OpenG7 — CA: Election Day Ops, Results & Audit (openg7-ca-election-day-ops-and-audit)

**Languages:** [English](#english) | [Français](#francais)

<a id="english"></a>

## English

**What this service does**  
Freeze and snapshot the voter list before the election, distribute it to polling places (poll pads/paper), support election‑day operations, then consolidate results with reconciliations and audit.

**Plain-language description**  
The day before, it **freezes the list** and sends it to polling places. On election day, it **helps teams find voters quickly**, then **gathers results**. Afterward, it **cross‑checks the numbers** and **keeps evidence** to show everything went well. In short: **make voting happen, count, verify**.

### Overview
- **OpenG7** public project. Code and configs here are **open-source**; production secrets and private endpoints live in a **separate private overlays repo**.
- **Contracts (schemas & APIs)** are defined in the reference repo: `openg7-electoral-systems-canada`.
- This service aims to be **transparent**, **auditable**, and **secure-by-default**.

### How to Run (dev)
1. Install prerequisites: Docker or your preferred runtime.
2. Copy a sample config from `config/samples/` to `config/dev.yaml` and edit as needed.
3. Run the service:
   ```bash
   # Example placeholder. Replace with your real entrypoint later.
   python -m app.main --config config/dev.yaml
   ```
4. Run tests:
   ```bash
   pytest -q
   ```

### Security
- No personal data (PII) should be committed to this repo.
- Secrets are managed via environment variables or secret stores (Vault, cloud KMS), **never** in Git.
- See **SECURITY.md** for responsible disclosure and hardening tips.

### Contributing
- Please read **CODE_OF_CONDUCT.md**.
- Open issues/PRs in English or French.
- Keep changes backward-compatible with published **contracts** when possible.

### License
Code: MIT © 2025 OpenG7 contributors.

---

<a id="francais"></a>

## Français

**Ce que fait ce service**  
Il **fige** et **prend un instantané** de la liste des électeurs avant le scrutin, la **distribue** aux lieux de vote (tablettes/papier), **soutient les opérations** du jour J, puis **consolide les résultats** avec des **réconciliations** et un **audit**.

**Description (grand public)**  
La veille, il **fige la liste** et l’envoie aux bureaux de vote. Le jour J, il **aide les équipes à retrouver les électeurs rapidement**, puis **rassemble les résultats**. Après, il **recoupe les chiffres** et **garde des preuves** pour montrer que tout s’est bien passé. En bref : **faire voter, compter, vérifier**.

### Aperçu
- Projet **OpenG7** public. Le code et les configs sont **open‑source** ; les secrets de production et les endpoints privés vivent dans un **repo d’overlays privé séparé**.
- Les **contrats (schémas & APIs)** sont définis dans le dépôt de référence : `openg7-electoral-systems-canada`.
- Ce service vise la **transparence**, l’**auditabilité** et la **sécurité par défaut**.

### Lancer en local (dev)
1. Installer les prérequis : Docker ou votre runtime préféré.
2. Copier un exemple de config depuis `config/samples/` vers `config/dev.yaml` et l’adapter.
3. Lancer le service :
   ```bash
   # Exemple de placeholder. Remplacez par votre point d’entrée réel.
   python -m app.main --config config/dev.yaml
   ```
4. Lancer les tests :
   ```bash
   pytest -q
   ```

### Sécurité
- Aucune donnée personnelle (PII) ne doit être commit dans ce dépôt.
- Les secrets sont gérés via variables d’environnement ou coffre (Vault, cloud KMS), **jamais** dans Git.
- Voir **SECURITY.md** pour la divulgation responsable et les conseils de durcissement.

### Contribution
- Merci de lire **CODE_OF_CONDUCT.md**.
- Issues et PRs en français ou en anglais.
- Rester compatible avec les **contrats** publiés quand c’est possible.

### Licence
Code : MIT © 2025 OpenG7 contributors.
