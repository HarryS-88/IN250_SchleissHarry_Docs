# Git Basics – Aufgabe 1

## Repository erstellen

Zuerst habe ich auf GitHub ein neues Repository erstellt.
Der Name des Repositories lautet IN250_SchleissHarry_Docs.

Das Repository ist öffentlich und wurde direkt mit einer README-Datei erstellt.

## Dokumentation mit Markdown

Anschliessend habe ich eine neue Markdown-Datei mit dem Namen git_basics.md
erstellt, in der ich meine Arbeitsschritte dokumentiere.



# Git Basics – Aufgabe 2

## Repository klonen

In dieser Aufgabe habe ich mein zuvor erstelltes Repository lokal auf meinen Computer geklont.

Zuerst habe ich Git Bash geöffnet und einen Ordner für die Schulunterlagen erstellt. Danach habe ich mit dem Befehl `git clone` mein Repository von GitHub auf meinen Computer kopiert.

Anschliessend bin ich in das geklonte Repository gewechselt und habe überprüft, ob alles korrekt funktioniert.

## Kontrolle

Zur Kontrolle habe ich folgende Befehle verwendet:
- `git status`
- `git remote -v`
- `git log --oneline`

Diese Befehle zeigen, dass das Repository korrekt geklont wurde, mit dem richtigen Remote verbunden ist und die Commit-Historie vorhanden ist.

# Git Basics – Aufgabe 3

## Markdown Cheatsheet ins Repository kopieren

In dieser Aufgabe habe ich mein zuvor erstelltes Markdown Cheatsheet in den Ordner meines geklonten Git-Repositories kopiert.

## Commit erstellen

Anschliessend habe ich die Änderungen mit einem Commit gespeichert.  
Die vorgegebene Commit-Nachricht lautete:
- `Initial commit`

# Git Basics – Aufgabe 4

## .gitignore erstellen

In dieser Aufgabe habe ich eine `.gitignore`-Datei in meinem Repository erstellt.

In dieser Datei habe ich definiert, dass alle Log-Dateien (`*.log`) sowie die Datei `GeheimeBankInformationen.txt` von Git ignoriert werden.

## Commit erstellen

Nach dem Erstellen der `.gitignore`-Datei habe ich die Änderungen mit einem Commit gespeichert.

Die Commit-Nachricht lautete:
- `Add gitignore`

# Git Basics – Aufgabe 5

## Zweites lokales Repository mit git init

In dieser Aufgabe habe ich in einem neuen Ordner ein weiteres lokales Git-Repository mit dem Befehl `git init` erstellt.

Anschliessend habe ich den Remote `origin` auf mein bestehendes GitHub-Repository gesetzt.

## Synchronisation mit dem Remote Repository

Nach dem Setzen des Remotes habe ich das lokale Repository mit `git pull origin main` mit dem GitHub-Repository synchronisiert.

Dabei wurden alle Dateien aus dem bestehenden GitHub-Repository in das neue lokale Repository übernommen.

## Beobachtung

Obwohl das neue Repository lokal leer war, wurde beim Pull ein neuer Branch erstellt und der komplette Inhalt vom Remote übernommen.

GitHub dient dabei als zentrale Quelle, mit der mehrere lokale Repositories synchronisiert werden können.

## Was passiert bei vorherigem Push?

Wenn im ursprünglichen lokalen Repository Änderungen vorgenommen und auf GitHub gepusht wurden, sind diese Änderungen im Remote vorhanden.

Beim anschliessenden `git pull` im neuen lokalen Repository werden diese Änderungen ebenfalls übernommen.

## Zusätzliche Beobachtung: Branch `master` vs. `main` (Repo2)

Beim Erstellen des zweiten lokalen Repositories mit `git init` war der Standard-Branch bei mir `master`.  
Mein GitHub-Repository verwendet jedoch den Branch `main`.

Nach dem `git pull origin main` wurden die Inhalte vom Remote heruntergeladen und der Branch `main` vom Remote wurde lokal angelegt.  
Meine Dokumentation zu Aufgabe 5 habe ich danach im Repo2 committed. Da ich mich dabei weiterhin auf dem Branch `master` befand, wurde beim Push ein neuer Remote-Branch `origin/master` erstellt.

Dadurch gibt es auf GitHub nun zwei Branches (`main` und `master`). GitHub zeigt deshalb den Hinweis **„Compare & pull request“** an.  
Ein Pull Request würde bedeuten, dass Änderungen von `master` in `main` zusammengeführt (gemerged) werden. Für diese Aufgabe war das nicht zwingend erforderlich, es zeigt aber, dass mehrere lokale Repositories auf dasselbe Remote arbeiten können und dabei unterschiedliche Branches entstehen können.
Ich erkenne dies auch daran, dass `git push` zuerst eine Upstream-Verknüpfung verlangte (Push mit `--set-upstream`), weil `master` noch keinen zugewiesenen Remote-Branch hatte.


# Git Basics – Aufgabe 6

## Warum Git in der Softwareentwicklung genutzt wird

Git wird in der Softwareentwicklung verwendet, um Änderungen am Code nachvollziehbar zu speichern und zu verwalten. Jede Änderung kann mit einem Commit dokumentiert werden, sodass jederzeit ersichtlich ist, wer was und wann geändert hat.

Ein weiterer wichtiger Vorteil von Git ist die Zusammenarbeit im Team. Mehrere Personen können gleichzeitig am gleichen Projekt arbeiten, ohne sich gegenseitig zu behindern. Über Branches lassen sich neue Funktionen oder Experimente getrennt entwickeln und später zusammenführen.

Zusätzlich bietet Git Sicherheit, da frühere Versionen jederzeit wiederhergestellt werden können. Falls ein Fehler gemacht wird, kann man auf einen früheren Stand zurückgehen.

---

## Warum bei einem Feuer zuerst Git Commit und Git Push erfolgen sollte

Der Vergleich mit einem Feuer soll verdeutlichen, wie wichtig es ist, Änderungen rechtzeitig zu sichern. Ein Git Commit speichert die aktuellen Änderungen lokal, ein Git Push sichert diese zusätzlich im Remote Repository (z. B. auf GitHub).

Falls der Computer beschädigt wird oder Daten verloren gehen, sind die letzten Änderungen durch den Push trotzdem noch vorhanden. Deshalb sollte man bei einem Notfall zuerst committen und pushen, bevor man den Arbeitsplatz verlässt.

So stellt Git sicher, dass wichtige Arbeit nicht verloren geht, selbst wenn unvorhergesehene Ereignisse eintreten.

# Git Basics – Aufgabe 7

## Dokumentation ins bestehende Repository integrieren

In dieser Aufgabe habe ich meine gesamte Dokumentation `git_basics.md` in mein bestehendes GitHub-Repository integriert.

Anschliessend habe ich die Änderungen mit einem Commit gespeichert und auf GitHub gepusht, sodass die vollständige Dokumentation zentral im Repository verfügbar ist.

Die Commit-Nachricht lautete:
- `Add git basics documentation`

## Projektdokumentation für Moodle

Zusätzlich habe ich die Projektstruktur sowie die Commit-Historie in einem Word-Dokument mit Screenshots dokumentiert und dieses anschliessend auf Moodle hochgeladen.
