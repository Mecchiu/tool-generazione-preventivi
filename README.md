Preventivi in Cantiere

Generatore di preventivi per imbianchino: compila i dati, aggiungi le voci di lavoro con un tap e ottieni un documento pronto da stampare o inviare via WhatsApp/Email.

Nato per un'esigenza concreta: sostituire i preventivi fatti a mano con uno strumento semplice, usabile dal cellulare, senza bisogno di competenze tecniche.

Come funziona

L'app è composta da un unico file HTML autosufficiente (index.html): niente build, niente dipendenze da installare, niente backend. Tutta la logica — calcolo dei totali, generazione del documento, salvataggio dei dati dell'azienda — gira nel browser.

Si compilano i dati dell'attività e del cliente (precompilati con un esempio, da modificare al primo utilizzo).
Si aggiungono le voci di lavoro tramite i pulsanti rapidi (tinteggiatura pareti, soffitto, stuccatura, verniciatura infissi, ecc.) oppure a mano, con quantità, unità di misura e prezzo unitario.
Si generano sconto, IVA (opzionale, utile per il regime forfettario) e note.
Si genera l'anteprima del documento, pronta per:
la stampa/salvataggio in PDF tramite il menu del browser;
la copia come testo formattato, da incollare direttamente in WhatsApp o Email.

I dati dell'azienda (nome, telefono, indirizzo) vengono salvati in locale nel browser (localStorage) così non servono reinserirli a ogni preventivo.

Stack tecnico
HTML, CSS, JavaScript vanilla — nessuna libreria esterna, nessun framework.
Nessun backend: tutta la logica è client-side.
Font da Google Fonts (IBM Plex Sans per l'interfaccia, Source Serif 4 per il documento stampato).
Deploy

Il progetto è pensato per essere ospitato come sito statico. Con GitHub Pages:

Impostazioni del repository → Pages.
Source: Deploy from a branch → branch main, cartella / (root).
Salva. Dopo circa un minuto il sito sarà raggiungibile all'indirizzo mostrato in quella pagina.

Non essendoci alcuna logica server-side, funziona identicamente su qualsiasi hosting statico gratuito (Netlify, Vercel, Cloudflare Pages).

Uso da mobile

Aprendo il link da smartphone e usando "Aggiungi a schermata Home" (Condividi su iOS, menu ⋮ su Android), lo strumento si comporta come un'app installata, senza bisogno di pubblicarlo su App Store o Play Store.

Limiti noti
I dati inseriti restano solo sul dispositivo su cui si usa l'app (nessuna sincronizzazione tra dispositivi diversi).
Il numero di preventivo è progressivo per dispositivo, non condiviso tra più telefoni/computer.
Nessuna gestione multi-utente o storico centralizzato dei preventivi: è pensato come strumento personale, non come gestionale.
