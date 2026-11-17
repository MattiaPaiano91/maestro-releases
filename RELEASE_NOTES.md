## 2026-11-17 — Versione 2.1.1: avvio stabile del motore desktop in WSL

- Mantenuto un processo `wsl.exe` come supervisore della sessione che ospita il motore desktop; evitato che WSL termini il daemon quando il launcher esce subito dopo `nohup`.
- Il lock di avvio viene rilasciato dopo la scrittura del PID, così una nuova finestra può rilevare e riusare il motore già attivo senza creare processi duplicati.
- Documentato il comportamento del supervisore e aggiunto il controllo del launcher alla suite desktop.

[Scarica Maestro per Windows](https://github.com/MattiaPaiano91/maestro-releases/releases/tag/v2.1.1)

Source-Commit: b72f5fbaaccb4fb39c306e365113b2da567bd560
