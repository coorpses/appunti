✨ ​ASP.NET Core
è un framework open-source, cross-platform per sviluppare applicazioni web e API sulla piattaforma .NET.
È l’infrastruttura che ti permette di:
- ricevere richieste HTTP
- elaborarle
- restituire risposte (HTML, JSON, file, ecc.)

✨ Differenza

<img width="487" height="185" alt="image" src="https://github.com/user-attachments/assets/654755b3-54f1-4597-81ab-407b66e86b0e" />

NET è la piattaforma su cui gira il codice.
- esegue il codice C#
- fornisce il runtime
- include le librerie fondamentali (stringhe, liste, file, date, thread…)
Ma da solo .NET non gestisce HTTP.

ASP.NET Core è uno strumento dentro .NET per fare applicazioni web. Aggiunge a .NET la capacità di:
- ascoltare richieste HTTP
- fare routing
- gestire API / controller
- rispondere a browser e app

**Esempio .NET:** Console.Writeline("ciao");
**Esempio ASP.NET:** app.MapGet("/ciao", () => "ciao");

Ci sono 3 tipi di progetto:
- ASP.NET Core Web App (Model-View-Controller) → MVC
- ASP.NET Core Web App → Razor Pages
- ASP.NET Core Web API → solo API, senza pagine web

✨ ​ASP.NET Core Web App MVC
- Controllers → logica (gestisce le richieste e decide cosa mostrare)
- Models → dati (classi / database)
- Views → pagine HTML
- Program.cs → configurazione principale

✨ Passare da una versione di .NET a una più nuova (es. da .NET 8 a .NET 10)
Quando passi da una versione di .NET a una più recente non cambia il modo di programmare di base, ma cambia il motore su cui gira l’applicazione
Cosa cambia in pratica:
- Prestazioni migliori (app più veloce e che usa meno memoria)
- Maggiore sicurezza (bug e vulnerabilità risolte)
- Nuove API e funzionalità disponibili
- Alcune API vecchie possono essere deprecate (da sistemare)

✨ Cos’è il .NET SDK (Software Development Kit)
È il pacchetto necessario per sviluppare applicazioni .NET. Senza SDK non puoi creare o compilare progetti.
Include:
- compilatore C#
- librerie base
- tool dotnet
- template di progetto (MVC, Web API, Razor Pages)
- runtime (serve solo per eseguire un’app già compilata tipo → eseguire un .exe o un’app compilata con dotnet publish)





