# Progettone website template
## Istruzioni per aggiungere il boilerplate del sito internet (website folder) alla cartella del progettone

1. Entra nella cartella del tuo progettone "my_progettone" e assicurati di non avere nella root una cartella che si chiama `website` in qeusto caso rinominala prima di proseguire:
  - `cd my_progettone`

3. Aggiungi il repository "progettone-template" come remoto al tuo repository "my_progettone":
  - `git remote add progettone-template https://github.com/sobigdata-master/progettone-template`


4. Recupera i file dal repository "progettone-template":
  - `git fetch progettone-template`


5. Imposta progettone-template come repository remoto
  - `git remote set-url origin https://github.com/sobigdata-master/progettone-template.git`


6. Mantieni il file readme.md del repository locale e ignora quello remoto (questo file che stai leggendo)
  - `git checkout --ours README.md`
  - `git add README.md`
  - `git commit -m "readme conflict resolved"`


7. Fai il merge dei file dal repository "progettone-template" e del tuo repository "my_progettone":
  - `git merge progettone-template/main --allow-unrelated-histories`


8. Fai il commit dei file appena aggiunti
  - `git commit -m "added jekyll boilerplate"`

9. Rimuovi il collegamento con il repository *progettone-template* (non più necessario)
  - `git remote remove progettone-template`

## La struttura della cartella dovrà avere una forma di questo tipo:
- code
- deliverables
- figures
- references
- **website**
readme.md
