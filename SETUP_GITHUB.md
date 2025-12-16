# Istruzioni per pubblicare su GitHub

## Step 1: Autenticazione GitHub CLI

Esegui questo comando per autenticarti:
```bash
gh auth login
```

Seguire le istruzioni per completare l'autenticazione.

## Step 2: Creare il repository

Dopo l'autenticazione, esegui uno di questi comandi:

### Opzione A: Creare nell'organizzazione "quality-and-safety"
```bash
gh repo create quality-and-safety/qualityandsafety-website --public --source=. --remote=origin --push
```

### Opzione B: Se il nome dell'organizzazione è diverso
Prima verifica il nome corretto dell'organizzazione:
```bash
gh org list
```

Poi crea il repository (sostituisci ORGANIZATION_NAME con il nome corretto):
```bash
gh repo create ORGANIZATION_NAME/qualityandsafety-website --public --source=. --remote=origin --push
```

### Opzione C: Creare manualmente su GitHub.com
1. Vai su https://github.com/organizations/quality-and-safety/repositories/new
2. Crea un nuovo repository chiamato `qualityandsafety-website`
3. Poi esegui questi comandi localmente:
```bash
git remote add origin https://github.com/quality-and-safety/qualityandsafety-website.git
git push -u origin main
```

## Repository già preparato

Il repository Git locale è già stato inizializzato con:
- ✅ Tutti i file del sito
- ✅ .gitignore configurato
- ✅ README.md
- ✅ Commit iniziale completato
- ✅ Branch principale rinominato in `main`

Non resta che pubblicarlo su GitHub!
