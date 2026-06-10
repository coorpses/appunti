✨ Angular​
---
Framewrok Javascript che permette di creare single paged applications (avviene tutto in una singola pagina, quindi quando cambio pagina NON rimando una richiesta, ma vengono mostrati diversi componenti in base a dove sono).
- Bisogna installare NODEJS (il runtime di javascript)
- Su VSCODE installare le estensioni per angular

✨ Progetto Angular​
---
<img width="200" height="400" alt="image" src="https://github.com/user-attachments/assets/d6d6bcaf-fcd9-4ec2-b37c-767d1f37c941" />

- .git e .vscode → file nascosti
- node_modules → gestore dei pacchetti di node → mostra la lista dei pacchetti installati
- .browserslistrc → file usato dal build per supportare i vari browser
- .editorconfig → si può specificare lo stile del codice
- .gitignore → file da ignorare su git (es. node_modules perchè troppo grande)
- angular.json → json con dati relativi ad angular
- karma.conf.js → serve per i test
- package.json → json con dati relativi al nostro progetto (es. nome, versione, script, dependencies)
- tsconfig.app.json → configurazione del typescript
- tsconfig.json → struttura di dati che serve al compilatore di typescript
- tsconfig.spec.json → serve per i test

✨ Cartella SRC​
---
Cartella app:
- app.module.ts → lista di componenti, moduli e services che usiamo
- app-routing.module.ts → gestisce il routing

Cartella assets:<br>
dove inserire i file che vogliamo usare, tipo immagini, pdf... <br>

Cartella environments:<br>
Ci sono 2 file, uno che riguarda l'ambiente di produzione e l'altro di development <br>

Index.html → componente root <br>
Main.ts → file da cui parte tutta l'applicazione angular <br>
Styles.css → css globale





