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

✨ Componenti​
---
```ts
import { Component } from '@angular/core'; 

@Component({     // decorator che serve per dire ad angular che questo è un componente
  selector: 'app-root',  // selettore che viene chiamato dentro l'html
  templateUrl: './app.component.html'
  styleUlrs: ['./app.component.css'] //array perchè può essercene più di uno
})
export class AppComponent {
  title = 'Nome componente';
}
```

✨ Data binding
---
Far comunicare il .ts con il suo .html. Ci sono 4 tipi di data binding:
- string interpolation (one-way)
- property binding (one-way)
- event binding (one-way)
- two way binding 

✨ String interpolation
---
Mostrare a schermo qualsiasi cosa che possa essere trasformato in una stringa
```html
<!-- HTML -->
<p> {{nome.ToUpperCase() }} </p>
<p> {{2 < 5? 'ciao' : 'hello' }} </p> 
```

✨ Property binding
---
```html
<!-- HTML -->
<button color="primary" [disabled]="isDisabled"> Cerca </button>
```
Possiamo bindare il funzionamento del bottone (se disabilitarlo o meno) aggiungendo le parentesi quadre all'attributo disabled. In questo modo disabled viene collegato alla variabile isDisabled che viene dal .ts

```ts
// TS
isDisabled = false;
```
✨ Event binding
---
```html
<!-- HTML -->
<button color="primary" (click)="onClick()"> Cliccami </button>
<input placeholder="Pizza" (input)="onInput($event)" />
```
```ts
// TS 
onInput(event: Event){ //mettere any non è il massimo
  console.log( (<HTMLInputElement>event.target).value ) } //prendo il valore che ho scritto nell'input
```
Ogni volta che io scrivo un carattere nell'input si genera un evento (dati). In questo modo angular sa già che, se scrivo $event,  voglio prendere tutto quell'insieme dei dati (si può vedere ispezionando l'evento).

✨ Two way binding
---
Collegare .ts e .html da entrambi i lati (mettere insieme property e event binding)
```html
<!-- HTML -->
<input placeholder="Pizza" [(ngModel)]="title" />
<p>{{title}}</p>
```
ngModel è una direttiva particolare che dice di connettere un evento sia in entrata che in uscita, quindi la variabile title potrà cambiare sia dall'.html che dal .ts, e la modifica viene vista da tutti e due (two way binding) <br>

✨ Direttive
---
Classi che vengono messe sugli elementi per andare a cambiare il comportamento degli elementi. Sono:
- built-in (ngModel, ngClass...)
- structural (*ngIf, *ngFor...) → modificano la struttura del DOM (html)
- attributi che modificano comportamento o apparenza di un elemento








