# Backups Manager

⚡ Gère vos fichiers de sauvegarde de manière intelligente.

## Fonctionnalités

Scanne votre dossier de fichiers de sauvegarde (sous le format `backupname-2020-08-01-1200.sql` par exemple) et applique les règles suivantes :

* Tous les fichiers des dernières 24 heures sont gardés.
* Un fichier par jour est gardé, pendant une semaine (celui créé à minuit).
* Un fichier par semaine est gardé, pendant un mois (celui créé le dimanche).
* Un fichier par mois est gardé, pendant un an (celui créé le premier du mois).

Les autres fichiers sont supprimés automatiquement.

## CronJob

CronJob pour exécuter automatiquement le script à une heure du matin:

```sh
0 1 * * * /usr/bin/ruby /path/to/backups_manager.rb
```
------------

### Translated to English

# Backup Manager

⚡ Manage your backup files intelligently.

## Features

Scans your backup files folder (in the format `backupname-2020-08-01-1200.sql` for example) and applies the following rules:

* All files from the last 24 hours are kept.
* One file per day is kept for a week (the one created at midnight).
* One file per week is kept for one month (the one created on Sunday).
* One file per month is kept for one year (the one created on the first of the month).

The other files are deleted automatically.

## [CronJob](https://www.google.com/search?q=cronjob+means)

CronJob to automatically run the script at one in the morning:

```sh
0 1 * * * /usr/bin/ruby /path/to/backups_manager.rb
```

