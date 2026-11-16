## 2026-11-16 — Versione 2.1.0: memoria selettiva e daemon persistente

- Sostituito il controllo Git globale con un coordinatore centrale e un watcher filesystem selettivo: durante il lavoro di agenti/subagenti il progetto è `Suspended`, mentre modifiche esterne successive invalidano soltanto le memorie collegate ai file il cui SHA-256 è cambiato.
- Separati e persistiti stato del monitor e stato della memoria; aggiunti freeze per progetto e interruttore globale, riattivazione con riconciliazione conservativa e blocco autoritativo di `memory_search` e `memory_get` per scope disabilitati, invalidati o non riconciliati.
- Introdotti riferimenti molti-a-molti tra memoria e file, migrazione dello schema 2.0, gestione di delete, rename, symlink e repository non Git e rimozione immediata degli embedding derivati dopo un'invalidazione.
- La panoramica dell'Aula mostra file e porzioni invalidate e offre eliminazione selettiva, eliminazione dell'intero progetto o rigenerazione esplicita tramite Memory Agent con prompt facoltativo. Gli avvisi ravvicinati sono aggregati e persistono con la UI chiusa.
- Il motore desktop resta attivo quando la UI viene chiusa, usa un lock di avvio e viene sostituito in sicurezza quando versione o protocollo del daemon non corrispondono; il supervisor di login Windows resta una scelta esplicita dell'installazione.
- Stabilizzato il menu azioni delle Aule durante gli aggiornamenti in background ed esclusi dai checkpoint i thread interni usati per generare i titoli.

Verifiche: 139 test Rust superati (2 prove reali escluse), 34 JavaScript, 9 del launcher desktop e 90 test browser end-to-end. Inclusi migrazione dello schema precedente, freeze globale/per progetto, invalidazione file-specifica, symlink interni/retarget esterni, filtro MCP autoritativo e check Tauri sul target Windows MSVC.

[Scarica Maestro per Windows](https://github.com/MattiaPaiano91/maestro-releases/releases/tag/v2.1.0)

Source-Commit: 90e73551328ff8968b2241726762cc753cc694c6
