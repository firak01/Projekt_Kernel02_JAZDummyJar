Merke: 
Verzeichnisse ohne Dateien werden nicht per Git übertragen.

Hinweis2: 
Binäre Dateien (also .jar) können nicht gemerged werden.
Bei einem Konflikt müssen diese per GitBash übertragen werden:

Also gitBash starten.
1. mit cd c:\\1fgl\\....... in den Ordner des Repository wechseln
2. Befehl: git reset HEAD relativer\\Pfad\\zur\\Datei
     oder    git reset master relativer\\Pfad\\zur\\Datei
3. Befehl: git checkout --theirs -- relativer\\Pfad\\zur\\Datei
    oder   git checkout --ours -- relativer\\Pfad\\zur\\Datei

Das reicht aber noch nicht aus.
Zusätzlich muss per Kommandozeile noch committed werden.
4. Befehl: git commit -a -m "wichtig den Kommentar nicht vergessen"