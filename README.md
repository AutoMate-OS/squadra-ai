# La squadra AI per Claude Code e Codex

Il modello della squadra che manda avanti un'azienda: un **office manager** che smista, **Marco** che prepara le risposte ai clienti, **Sara** che prepara i solleciti, **Elena** che segue i preventivi. Tutti lavorano su bozze: non inviano mai niente senza il tuo ok. Funziona dentro la **cartella della tua azienda** (contesto, ruoli, memoria delle correzioni).

## Come si usa (due minuti)

1. Scarica questo repository (**Code → Download ZIP**, oppure `git clone`).
2. Apri la cartella con **Claude Code** o con **Codex**.
3. Scrivi: **"Crea la squadra AI della mia azienda"**.
   - In Claude Code parte la skill `crea-squadra-ai`. In Codex segue `AGENTS.md`.
   - Ti fa alcune domande e crea **una nuova cartella** con la tua squadra, partendo dal modello in `modello/`.
4. Apri la **nuova** cartella: gli agenti sono già pronti (`.claude/agents/` per Claude Code, `.codex/agents/` per Codex).

Se preferisci farlo a mano, copia `modello/` e sostituisci `[NOME AZIENDA]` e gli esempi.

## Cosa c'è dentro

```
modello/
├── AGENTS.md              ← chi siamo, regole, la squadra (per Codex; Claude lo importa da CLAUDE.md)
├── CLAUDE.md
├── correzioni.md          ← la memoria: ogni tua correzione finisce qui
├── ruoli/office-manager.md
├── .claude/agents/        ← marco-posta, sara-incassi, elena-vendite (Claude Code)
├── .codex/agents/         ← gli stessi tre in formato Codex (.toml)
└── dati/                  ← listino, condizioni, clienti, mail buone
```

## Sicurezza e privacy

- La skill **non usa la rete**, non invia dati a nessuno e **non cancella né sovrascrive** file: scrive solo nella nuova cartella che le indichi.
- Gli agenti del modello **preparano bozze e non inviano mai**; le richieste sospette (per esempio il cambio di IBAN) le girano a te.
- Nel modello ci sono solo esempi inventati. Non pubblicare mai la cartella compilata: contiene i tuoi clienti.
- Prima di dare a Claude o a Codex il link a un repository, leggi cosa contiene: qui sono file di testo, tutti leggibili.

## Vuoi che la montiamo noi?

Contesto, ruoli, memoria, collegamento con la tua posta e il tuo gestionale, e le automazioni quando le bozze escono giuste. Scrivi ad **alex@automate-pro.com** o vai su **automate-pro.com**.

Licenza MIT. Vedi anche: [cartella-azienda](https://github.com/AutoMate-OS/cartella-azienda).
