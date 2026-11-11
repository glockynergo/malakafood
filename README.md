# Malakafood

Sito dimostrativo di un ristorante, realizzato con **React 19 e Vite**.

## Avvio

```sh
npm ci
npm run dev
```

## Build

```sh
npm run build
npm run preview
```

La build statica è in `dist/` e può essere distribuita su qualsiasi hosting statico.

## Funzioni

- Home con CTA Contattaci in evidenza e menu mobile.
- Animazione iniziale, ingressi allo scorrimento e interazioni sui bottoni.
- Galleria filtrabile e lightbox con navigazione da tastiera.
- Modulo contatti dimostrativo con validazione: non invia né salva dati.
- Responsive e supporto a `prefers-reduced-motion`.

Recapiti lasciati vuoti su richiesta. Immagini illustrative Unsplash, scaricate localmente; caratteri Google Fonts. Nessun indirizzo, orario o recapito fittizio. Per attivare contatti reali occorre aggiungere un recapito o un servizio di invio e aggiornare il modulo.

## Pubblicazione su GitHub Pages

Sito: https://glockynergo.github.io/malakafood/

Il workflow `.github/workflows/deploy-pages.yml` compila e pubblica il sito a ogni push su `main`. In **Settings → Pages → Build and deployment**, la sorgente deve essere **GitHub Actions**.

Per riprodurre la build Pages localmente:

```sh
VITE_BASE_PATH=/malakafood/ npm run build
```

La configurazione predefinita conserva `/` come percorso base per sviluppo e altri hosting. Tutte le immagini utilizzano il percorso base configurato.
