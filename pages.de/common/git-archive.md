# git archive

> Erstelle ein Archiv von Dateien.
> Weitere Informationen: <https://git-scm.com/docs/git-archive>.

- Erstelle ein tar-Archiv aus dem Inhalt des aktuellen HEAD und gib dieses aus:

`git archive {{[-v|--verbose]}} HEAD`

- Erstelle ein zip-Archiv aus dem Inhalt des aktuellen HEAD und gib dieses aus:

`git archive {{[-v|--verbose]}} --format zip HEAD`

- Erstelle ein zip-Archiv aus dem Inhalt des aktuellen HEAD und speichere dieses in eine Datei:

`git archive {{[-v|--verbose]}} {{[-o|--output]}} {{pfad/zu/datei.zip}} HEAD`

- Erstelle ein tar-Archiv aus dem Inhalt des letzten Commits eines bestimmten Branches:

`git archive {{[-o|--output]}} {{pfad/zu/datei.tar}} {{branch_name}}`

- Erstelle ein tar-Archiv aus dem Inhalt eines bestimmten Verzeichnisses:

`git archive {{[-o|--output]}} {{pfad/zu/datei.tar}} HEAD:{{pfad/zu/verzeichnis}}`

- Stelle jeder Datei einen Pfad voran, um sie in einem bestimmten Verzeichnis zu archivieren:

`git archive {{[-o|--output]}} {{pfad/zu/datei.tar}} --prefix {{pfad/zu/verzeichnis}}/ HEAD`
