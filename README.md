# andreaferalo.com

Sito ufficiale di **Andrea Feralo**, scrittore italiano.

## ✦ Caratteristiche

- Design letterario scuro ed elegante
- Tipografia raffinata (Cinzel + Cormorant Garamond)
- Effetto libro 3D interattivo
- Animazioni di scroll reveal
- Completamente responsive (mobile, tablet, desktop)
- Pronto per GitHub Pages (deploy statico)

## 📁 Struttura del Progetto

```
andreaferalo/
├── index.html          # Pagina principale
├── css/
│   └── style.css       # Stili (dark literary theme)
├── js/
│   └── main.js         # Interazioni e animazioni
├── images/             # Cartella per immagini (foto autore, copertine)
└── README.md
```

## 🚀 Deploy su GitHub Pages

### Metodo 1 — Tramite GitHub Web

1. Crea un repository su GitHub (es. `andreaferalo`)
2. Carica tutti i file tramite il pulsante **"Add file → Upload files"**
3. Vai in **Settings → Pages**
4. In "Branch" seleziona `main` e root `/`
5. Clicca **Save** → il sito sarà live su `https://tuo-username.github.io/andreaferalo`

### Metodo 2 — Tramite Git da terminale

```bash
# Inizializza il repository locale
git init
git add .
git commit -m "Prima versione del sito"

# Collega al repository remoto su GitHub
git remote add origin https://github.com/TUO-USERNAME/andreaferalo.git
git branch -M main
git push -u origin main

# Poi attiva GitHub Pages in Settings → Pages
```

### Dominio personalizzato (andreaferalo.com)

Dopo aver attivato GitHub Pages:

1. Crea un file `CNAME` nella root con il contenuto: `andreaferalo.com`
2. Dal tuo provider DNS, aggiungi questi record:
   ```
   A     @    185.199.108.153
   A     @    185.199.109.153
   A     @    185.199.110.153
   A     @    185.199.111.153
   CNAME www  tuo-username.github.io
   ```
3. In **Settings → Pages → Custom domain** inserisci `andreaferalo.com`

## 🖼️ Personalizzazione

### Aggiungere la foto dell'autore

1. Carica la foto in `/images/autore.jpg`
2. In `index.html`, sostituisci il blocco `.portrait-placeholder` con:
   ```html
   <img src="images/autore.jpg" alt="Andrea Feralo" style="width:260px; height:340px; object-fit:cover; border: 1px solid rgba(201,168,76,0.2);" />
   ```

### Aggiungere la copertina del libro

1. Carica la copertina in `/images/debito-anima.jpg`
2. Nel CSS, imposta `.book-cover-art` con `background-image: url('../images/debito-anima.jpg')`

### Modificare i testi

Tutti i contenuti testuali si trovano in `index.html` e sono facilmente identificabili.

---

© 2025 Andrea Feralo · Tutti i diritti riservati
