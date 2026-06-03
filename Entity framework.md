✨ ORM
---
Un Object-Relational Mapper fornisce un livello di astrazione interposto tra l’applicazione e il database che:
- semplifica le operazioni di interrogazione e manipolazione dei dati
- implementa l’indipendenza dall'origine dei dati: cambiare DBMS non implica modificare il
codice che lo usa.

In poche parole ti permette di lavorare col database (interrogare e modificare i dati) usando classi C# invece che SQL a mano.

✨ Entity Framework (EF)
---
è un ORM sviluppato da Microsoft, open source e scaricabile come pacchetto NuGet.

✨ EF provider
---
è uno “strato” di software che si interpone tra EF e il DBMS con il quale deve
dialogare. Dunque, EF non è utilizzabile con quei DBMS per i quale non esiste un EF provider (es. access).
Permette di progettare l'entity model.

✨ Domain model (entity model)
---
Esempio di una entity model, composta da due classi, Cliente e Ordine
<img width="756" height="308" alt="immagine" src="https://github.com/user-attachments/assets/807016bf-c2f6-4200-be54-3f69402fe4c0" />
