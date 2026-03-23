# Memoria progetto — Sito IFL-Network
*Generata il 23 marzo 2026*

---

## Situazione di partenza

- Sito attuale: **ifl-network.it** costruito con **IONOS MyWebsite Pack Plus**
- Costo: **18€/mese** (pagamento mensile, disdetta possibile in qualsiasi momento)
- Il piano include hosting + dominio in un unico pacchetto (non separabili)
- Email aziendale **info@ifl-network.it** già migrata su **Google Workspace** (pagato separatamente)
- I record MX (email) sono configurati su IONOS e puntano a Google — non dipendono dall'hosting

---

## Decisioni prese

### Obiettivo
Abbandonare IONOS e ridurre i costi a ~12€/anno (solo rinnovo dominio).

### Soluzione scelta
- **Hosting:** GitHub Pages (gratuito)
- **Dominio:** da tenere su IONOS con piano solo-dominio (~12€/anno) dopo la migrazione
- **Email:** nessun cambiamento — rimane su Google Workspace
- **Analytics:** da configurare con Google Analytics 4 (gratuito)
- **SEO:** da configurare con Google Search Console (gratuito)

### Risparmio stimato
~200€/anno

---

## Estetica del sito

### Palette colori scelta — Opzione A: Blu professionale

| Ruolo | Colore | Hex |
|---|---|---|
| Colore principale (navbar, hero, footer) | Blu scuro | `#1E3A5F` |
| Colore secondario (bottoni, accenti) | Blu medio | `#2E6DB4` |
| Sfondo chiaro | Azzurro pallido | `#E8F1FB` |
| Sfondo pagina | Grigio chiarissimo | `#F4F6F9` |
| Bordi | Grigio-blu | `#D0D8E4` |

### Struttura sito
- Pagina unica con scroll (homepage + servizi + contatti)
- Navbar fissa in alto
- Hero section con titolo e CTA
- 4 card servizi con icone SVG (no foto)
- Sezione contatti con mappa
- Footer

---

## Infrastruttura tecnica

### Account creati
- **GitHub:** github.com/giacomoluzzi

### Repository
- URL: `https://github.com/giacomoluzzi/ifl-network`
- Branch principale: `main`
- GitHub Pages attivo → sito live su: `https://giacomoluzzi.github.io/ifl-network`

### Struttura cartella locale
```
C:\Users\Giacomo\Documents\IFL-Network\Website\
├── index.html
└── images/        ← da creare quando servono immagini
```

### Configurazione Git
```bash
git config --global user.name "Giacomo Luzzi"
git config --global user.email "[tua email GitHub]"
```

---

## Flusso di lavoro per modificare il sito

1. Apri VS Code nella cartella `Website`
2. Modifica `index.html`
3. **Ctrl + S** per salvare
4. Nel terminale:
```bash
git add .
git commit -m "descrizione della modifica"
git push
```
5. Aspetta 1-2 minuti → il sito si aggiorna automaticamente

---

## Prossimi step da completare

- [ ] Aggiungere logo nella navbar (salvare in `images/`, richiamare con `<img src="images/logo.png">`)
- [ ] Aggiungere mappa Google Maps nella sezione contatti
- [ ] Configurare **Google Analytics 4** (incollare script nell'`<head>` di index.html)
- [ ] Configurare **Google Search Console** (verifica proprietà dominio)
- [ ] Trasferire il dominio `ifl-network.it` su piano solo-dominio IONOS
- [ ] Puntare il dominio verso GitHub Pages (record DNS su IONOS)
- [ ] Disdire il piano IONOS MyWebsite Pack Plus
- [ ] Aggiornare copyright footer da 2025 a anno corrente se necessario

---

## Note tecniche utili

### Ottimizzazione immagini
Usare **squoosh.app** (gratuito, browser) per ridurre il peso delle immagini prima di caricarle.

### Attenzione nomi file
Su GitHub Pages il server è case-sensitive (Linux). Usare sempre **nomi minuscoli** per i file:
- ✅ `index.html`, `logo.png`
- ❌ `Index.html`, `Logo.PNG`

### Comando utile se Git non riconosce rinomina maiuscole/minuscole
```bash
git mv NomeFile.html nomefile.html
git commit -m "rinominato in minuscolo"
git push
```

---

## Contenuto attuale del sito (da index.html)

### Headline
"Affianchiamo le aziende con strumenti su misura"

### Sottotitolo
"Affrontiamo in modo diretto le esigenze delle aziende, mirando ai risultati richiesti e supportandole con strumenti informatici creati ad hoc."

### Servizi
1. **Certificazioni** — ISO 9001 Qualità, ISO 14001 Ambiente, ISO 45001 Sicurezza
2. **Sicurezza in azienda** — Monitoraggio macchine e luoghi di lavoro
3. **Controllo di gestione** — Prestazioni economiche e progetti di investimento
4. **Brevetti industriali** — Elaborazione domande di brevetto

### Contatti
- Indirizzo: Via Ponchielli, 32 — 23900 Lecco (LC)
- Email: info@ifl-network.it
- Tel: +39 331 389 1023 / +39 338 634 4444
