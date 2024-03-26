# progettone website template
## istruzioni per aggiungere il progetto del sito internet (website folder) alla cartella del progettone

1. Entra nella cartella del tuo progettone "my_progettone":
  - `cd my_progettone`

3. Aggiungi il repository "progettone-template" come remoto al tuo repository "my_progettone":
  - `git remote add progettone-template https://github.com/sobigdata-master/progettone-template`


4. Ora puoi recuperare i file dal repository "progettone-template" al tuo locale:
  - `git fetch progettone-template`


5. Imposta progettone-template come repository remoto
  - `git remote set-url origin https://github.com/sobigdata-master/progettone-template.git`


6. Rimuovi il file readme.md dal repository locale
  - `git rm README.md`
  - `git commit -m "removed readme.md"`


7. Fai il merge dei file dal repository "progettone-template" al tuo repository "my_progettone":
  - `git merge progettone-template/master --allow-unrelated-histories`


8. Aggiorna il tuo repository remoto con la cartella website appena scaricata.

## la struttura della cartella dovrà avere una forma di questo tipo:
- code
- deliverables
- figures
- references
- **website**
