## 2026-11-14 — Versione 2.0.0: memoria condivisa e interoperabilità

- Introdotta la memoria di progetto condivisa fra Aule, con persistenza e ricerca vettoriale locali, fonti, revisioni e un indice leggero nel progetto. Il consolidamento e gli embedding usano servizi API configurabili.
- Aggiunti i tool MCP di ricerca e consultazione scoped per progetto e la loro configurazione nelle sessioni Codex e ACP. Il supporto delle CLI reali dipende dal runtime installato; Pi richiede un'estensione dedicata.
- Collegati checkpoint a fine turno, cambio agente, archiviazione e interruzione, con cursori persistenti e recupero dei checkpoint interrotti.
- Bloccata la consultazione durante sincronizzazioni e modifiche Git non elaborate; aggiunti nell'Aula stato, file modificati e azioni di sincronizzazione o disabilitazione.
- Aggiunte nelle impostazioni la configurazione dei servizi memoria ed embedding e la verifica delle connessioni. Le chiavi restano fuori dal database e non vengono restituite alla UI.
- Estesa l'interoperabilità a nove provider con capability dichiarate, controlli UI coerenti e matrice di compatibilità; le integrazioni senza runtime reale restano da verificare.
- Rafforzati il rilevamento delle modifiche ripetute ai file, la coerenza tra checkpoint e revisioni e la protezione delle chat isolate dall'accesso a server MCP esterni.

[Scarica Maestro per Windows](https://github.com/MattiaPaiano91/maestro-releases/releases/tag/v2.0.0)

Source-Commit: 7c3a56f56ec5b33a8093a87fa7af3b442dc43705
