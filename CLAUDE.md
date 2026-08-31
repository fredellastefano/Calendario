# Istruzioni per i commit su questo repository

- Nei commit git su questo repository, l'autore (Author e Committer) deve
  sempre essere l'utente proprietario del progetto, non "Claude" o altri
  riferimenti ad Anthropic/Claude Code:
  - Author: `Stefano Fredella <fredella.stefano@gmail.com>`
  - Committer: `Stefano Fredella <fredella.stefano@gmail.com>`
- Non includere nei messaggi di commit trailer come `Co-Authored-By: Claude`,
  `Claude-Session:`, o qualsiasi altro riferimento a Claude/Anthropic.
- Per impostare l'autore/committer corretto senza modificare la
  configurazione globale di git, usare variabili d'ambiente ed il flag
  `--author` solo per il singolo commit, ad esempio:

  ```
  GIT_COMMITTER_NAME="Stefano Fredella" GIT_COMMITTER_EMAIL="fredella.stefano@gmail.com" \
  git commit --author="Stefano Fredella <fredella.stefano@gmail.com>" -m "messaggio"
  ```
