## 2026-11-18 — Versione 2.1.5: link desktop, marchio e rifiniture UI

- I link della chat, delle attività e dei terminali aprono gli URL nel browser di sistema. I file Windows e WSL si aprono nell’app associata; i percorsi relativi sono risolti nella cartella del progetto. Gli errori per file mancanti e anteprime private di altri client vengono mostrati nella UI.
- Conservati i collegamenti Markdown ai file e rese cliccabili le immagini Markdown senza caricare contenuti remoti nella chat. Rimossi i riferimenti di riga prima dell’apertura; protocolli eseguibili rifiutati e accesso al comando desktop limitato alla finestra principale e all’origine del motore corrente.
- Marchio M maiuscola bianca dal tratto sottile con il libro sottostante, condiviso da favicon, icone desktop, schermata di avvio e controlli. Sidebar con nome Maestro e libro; rimossa l’icona aggiuntiva dalla barra superiore desktop.
- Sidebar Attività dell’Aula estesa fino al bordo superiore anche nel desktop; conservati allineamenti e scorrimento.
- Rimossi la riga di stato sotto il composer e il logo accanto al pulsante +. Pulsanti Attività e Terminale con contorno e larghezza coerenti.

Verifiche prima della promozione: controlli JavaScript, test Rust e desktop, test browser mirati e build Windows; verificati anche sul desktop Windows reale il bridge nativo, l’apertura nel browser di sistema, i percorsi Windows/WSL/relativi e gli errori visibili. L’aggiornamento deve essere installato: la vecchia app continua a usare il motore e il renderer precedenti fino al riavvio con la nuova versione.

[Scarica Maestro per Windows](https://github.com/MattiaPaiano91/maestro-releases/releases/tag/v2.1.5)

Source-Commit: 5d4c4f073fdc3f7f4f9aeff6f3305727a06a5571
