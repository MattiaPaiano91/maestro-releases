## 2026-11-14 — Versione 1.3.0: integrazione delle funzionalità multiagente

- Automatizzato il rilascio completo al push su `main`, con test, build, firma, tag, release GitHub e verifica del manifest pubblico; conservati controlli e artifact di prova su `develop`, pull request e avvii manuali.
- Aggiunte protezioni per versioni incoerenti o riutilizzate, commit superati, pacchetti immutabili e ripresa delle pubblicazioni interrotte. Esplicitato il flusso automatico in `AI_CONTRACT.md`.
- Consolidati runtime multiagente, Aule, handoff, note e API della memoria nella linea di sviluppo condivisa di Maestro.
- Importate le ultime modifiche del ramo `feature/agent-ui-capabilities`: controlli basati sulle capacità degli agenti, creazione guidata delle Aule, eliminazione confermata delle note e logging strutturato con rotazione.
- Allineate a 1.3.0 le versioni del motore, del desktop e dei lockfile prima della promozione da `develop` a `main`.
- Corretta la sincronizzazione dello stato: una risposta HTTP ritardata conserva gli eventi più recenti di turni, autorizzazioni e notifiche, e non sostituisce uno stato già caricato da una richiesta successiva.
- Conservata la posizione di lettura quando arrivano i controlli del modello e dello sforzo: le chat aperte in fondo restano sull'ultimo messaggio anche aprendo il terminale.
- Riallineati i test browser alla navigazione per Aule e al composer adattivo; resi deterministici il posizionamento del cursore e gli eventi controllati dai test.

Verifiche: 125 test Rust superati (2 prove reali escluse), 33 JavaScript e 6 del launcher desktop. Validati i workflow con actionlint e testate senza pubblicazioni reali le protezioni di versione, firma, provenienza e immutabilità dei pacchetti. Eseguita la suite browser di 87 casi; dopo l'allineamento dei mock, superati tutti i 18 test della dashboard e le riesecuzioni mirate su autorizzazioni e scorrimento. Build release Linux e installer Windows completate, con firma degli aggiornamenti verificata.

[Scarica Maestro per Windows](https://github.com/MattiaPaiano91/maestro-releases/releases/tag/v1.3.0)

Source-Commit: 7af1a2c4ad2a86287953473191e37a13120b5017
