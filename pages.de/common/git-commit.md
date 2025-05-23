# git commit

> Committe Dateien in ein Repository.
> Weitere Informationen: <https://git-scm.com/docs/git-commit>.

- Committe die gestagten Dateien mit einer Nachricht in das Repository:

`git commit {{[-m|--message]}} "{{nachricht}}"`

- Committe alle gestagten Dateien zum Repository mit einer Nachricht aus einer Datei:

`git commit {{[-F|--file]}} {{pfad/zu/commit_nachricht_datei}}`

- Stage alle modifizierten Dateien und committe sie mit einer Nachricht:

`git commit {{[-a|--all]}} {{[-m|--message]}} "{{nachricht}}"`

- Committe gestagten Dateien und signiere sie mit dem definierten GPG Schlüssel (oder mit dem in der Konfigurationsdatei definierten, wenn kein Argument angegeben ist):

`git commit {{[-S|--gpg-sign]}} {{key_id}} {{[-m|--message]}} "{{nachricht}}"`

- Ersetze den letzten Commit mit den gerade auf dem Stage liegenden Änderungen:

`git commit --amend`

- Comitte nur spezifische Dateien (die Dateien müssen schon auf dem Stage liegen):

`git commit {{pfad/zu/datei1 pfad/zu/datei2 ...}}`

- Erzeuge einen Commit, auch wenn keine Dateien auf dem Stage liegen:

`git commit {{[-m|--message]}} "{{nachricht}}" --allow-empty`
