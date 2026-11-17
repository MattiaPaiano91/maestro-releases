## 2026-11-17 — Versione 2.1.2: dati Maestro indipendenti dall’agente

- Le sessioni scomparse dall’elenco Codex non vengono più eliminate dal catalogo Maestro: restano collegate all’Aula, marcate come non disponibili e tornano normali se il provider le espone di nuovo.
- Le Aule conservate vengono mostrate anche quando il payload della sessione nativa non è più disponibile, evitando il conteggio senza righe corrispondenti.
- Aggiunto l’archivio globale **Note Maestro**, con lettura e modifica delle note anche quando la conversazione originale non esiste più.
- Le API delle note non richiedono più che il thread nativo sia presente nel catalogo; eliminazione esplicita della conversazione ed eliminazione dei dati Maestro restano operazioni distinte.
- Aggiornato il contratto del progetto per impedire che configurazioni o credenziali di un provider cancellino o nascondano Aule e note.

[Scarica Maestro per Windows](https://github.com/MattiaPaiano91/maestro-releases/releases/tag/v2.1.2)

Source-Commit: ca58be4ec404edf318e61832748d5cad300dc76f
