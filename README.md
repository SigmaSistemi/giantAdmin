# giantAdmin

Pagina web per l'installazione di GiantAdmin

https://sigmasistemi.github.io/giantAdmin

Il codice sorgente è nel repository privato `SigmaSistemi/GiantAdmin.WPF`.

## Come funziona

L'app usa [Velopack](https://velopack.io) per installazione e auto-update. Ad ogni nuova versione
pubblicata (push su `main` nel repo privato `GiantAdmin.WPF` con `<Version>` incrementata nel
`.csproj`), il workflow di quel repo compila l'app e pubblica una **GitHub Release** qui, con tag
`vX.Y.Z` e come asset l'installer `SigmaSistemi.GiantAdmin-win-Setup.exe` più i pacchetti di
update usati da Velopack per gli aggiornamenti automatici (`RELEASES`, i `.nupkg`, ecc.).

La pagina `index.html` punta sempre a `.../releases/latest/download/SigmaSistemi.GiantAdmin-win-Setup.exe`,
quindi non va aggiornata manualmente ad ogni release: il link "latest" di GitHub segue da solo
l'ultima versione pubblicata.

Non serve mai intervenire a mano su questo repo per pubblicare una release.

