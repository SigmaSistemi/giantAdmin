# giantAdmin

Pagina web per l'installazione di GiantSQL Administrator

https://sigmasistemi.github.io/giantAdmin

Il codice sorgente è nel repository privato `SigmaSistemi/GiantAdmin.WPF`.

## Pubblicare una nuova versione

1. Nel repo `GiantAdmin.WPF`, compila in Release x64 e genera l'installer con Inno Setup (`installer/GiantAdmin.iss`), ottenendo `installer/dist/GiantAdmin_setup.exe`.
2. Copia il nuovo `GiantAdmin_setup.exe` qui in questo repo, sovrascrivendo quello esistente.
3. Commit e push su `main`: la pagina si aggiorna automaticamente (GitHub Pages, branch `main`, root).

