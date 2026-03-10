# Conspirators.blog — Guida al setup

## Struttura del progetto

```
conspirators/
├── index.html              ← Homepage del blog
├── netlify.toml            ← Configurazione Netlify
├── static/
│   └── admin/
│       ├── index.html      ← Pannello CMS (Decap CMS)
│       └── config.yml      ← Configurazione CMS
├── content/
│   └── posts/              ← I tuoi articoli in Markdown
└── static/
    └── images/             ← Immagini caricate dal CMS
```

---

## Setup passo per passo

### 1. Crea repository GitHub
1. Vai su [github.com](https://github.com) → **New repository**
2. Nome: `conspirators-blog`
3. Visibilità: **Public** (necessario per il piano gratuito Netlify)
4. Clicca **Create repository**

### 2. Carica i file su GitHub
Trascina tutti i file di questa cartella nel repository GitHub appena creato.

### 3. Crea account Netlify
1. Vai su [netlify.com](https://netlify.com)
2. **Sign up with GitHub**
3. Clicca **Add new site → Import an existing project**
4. Seleziona **GitHub** → scegli `conspirators-blog`
5. Build settings: lascia tutto vuoto (sito statico)
6. Clicca **Deploy site**

### 4. Collega il tuo dominio
1. In Netlify: **Domain settings → Add custom domain**
2. Inserisci `conspirators.blog`
3. Netlify ti darà i nameserver da impostare nel pannello del tuo registrar

### 5. Attiva Netlify Identity (per il CMS)
1. In Netlify: **Site settings → Identity → Enable Identity**
2. Scorri fino a **Git Gateway** → clicca **Enable Git Gateway**
3. Vai su **Identity → Invite users** e invita la tua email

### 6. Accedi al pannello admin
1. Vai su `conspirators.blog/admin/`
2. Accetta l'invito email
3. Inizia a scrivere i tuoi articoli! 🔴

---

## Come pubblicare un articolo

1. Vai su `/admin/`
2. Clicca **Nuovo articolo**
3. Compila: titolo, categoria, estratto, tag, contenuto
4. Clicca **Pubblica**
5. Il sito si aggiorna automaticamente entro 1-2 minuti

---

## Costi

| Servizio | Piano | Costo |
|---|---|---|
| GitHub | Free | €0/mese |
| Netlify | Starter | €0/mese |
| Dominio | .blog | ~€30/anno |

**Totale: ~€30/anno** (solo il dominio)
