# giantAdmin

Pagina web per l'installazione di GiantAdmin

https://sigmasistemi.github.io/giantAdmin

Il codice sorgente è nel repository privato `SigmaSistemi/GiantAdmin.WPF`.

## Pubblicare una nuova versione

**Automatico**: ad ogni push su `main` nel repo privato `GiantAdmin.WPF`, il workflow `build-and-publish.yml` compila l'app, genera l'installer con Inno Setup e pusha il nuovo `GiantAdmin_setup.exe` direttamente qui — non serve intervenire a mano.

Se dovesse servire un aggiornamento manuale: copia il nuovo `GiantAdmin_setup.exe` in questo repo (sovrascrivendo quello esistente) e fai commit/push su `main`.

