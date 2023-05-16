# GitLab für Texte - Tutorial


## Welche Texte werden hier betrachtet?

Hier nur ein paar Beispiele für Texte im Bereich Bildung und Wissenschaft. Weitere Gebiete, in denen mit Texten oder Projekten gearbeitet wird, sind natürlich ebenso denkbar ;-)

### Schule

* Unterrichtsvorbereitungen [Vorlage]()
* Skripte mit Anleitungen und Übungen
* Klausurvorbereitungen

### Studium

* Projektarbeiten
* Studienarbeiten
* Bachelorarbeiten
* Masterarbeiten

### Wissenschaft

* Doktorarbeiten
* Veröffentlichungen
* Projektdokumentation


## Was ist GitLab?

GitLab ist eine Webanwendung für die  Versionsverwaltung von - ursprünglich - Software Projekten auf der Basis von Git. [Wikipedia](https://de.wikipedia.org/wiki/GitLab)

Was hat das mit Bildung zu tun? Nicht jeder programmiert! Mit GitLab lassen sich auch Texte für Bildungsmaterialen, Studienarbeiten u.v.a.m. verwalten, gemeinsam bearbeiten und multimedial veröffentlichen - **ohne Kosten, ohne Installation, ohne Infrastruktur**!

GitLab bietet

* Plattform für die Verwaltung von (Text) Projekten
* Hosten von Webseiten
* Versionskontrolle
* Benutzermanagement für Projekte
* Projektmanagement

Mit einem kostenlosen Account auf GitLab lassen sich Projekte in Dateiverzeichnissen online verwalten. Vergleichbar mit einer Dropbox, aber mit vielen weiteren Funktionen, wie Versionierung, Automatisierung und Benutzer- und Rechteverwaltung.

Und so sieht das ganze in der Praxis aus ...

<iframe width="560" height="315" src="https://www.youtube.com/embed/i8MxZU9w6bc" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen="allowfullscreen"></iframe>

Beispiele

* [Ein Beispiel Kurs](https://gitlab.com/TIBHannover/oer/course-metadata-test)
* [Eine Beispiel Studienarbeit](https://gitlab.com/axel-klinger/studienarbeit)


## Ein erstes Projekt - Mein erster Kurs


Mit den folgenden Schritten erstellt man einen Kurs in GitLab.

* [Registrierung/Anmeldung](https://gitlab.com/users/sign_in)
* Projekt anlegen (+ in der Kopfzeile)
  - Name: freie Bezeichnung, präzise und einprägsam
  - Public, um für andere sichtbar zu sein
  - README anlegen, sonst ENTWICKLER-HÖLLE ;-)
* Dokument im Projekt anlegen (+ in der Mitte)
* reinschreiben, wie der Kurs heißt und einen Absatz als Einleitung

Und hier das ganze nochmal im Video ...

<iframe width="560" height="315" src="https://www.youtube.com/embed/7vmyyFigXPQ" frameborder="0" allow="accelerometer" allowfullscreen="allowfullscreen"></iframe>


## Ein zweites Projekt aus Vorlage - Mein erster OER Kurs

### Vorteile

* Ausgabeformate HTML, PDF und EPUB (u.v.a.m.)
* TULLU Kennzeichnung von Wikimedia Commons Bildern
* Maschinenlesbare Metadaten zur Auffindbarkeit
* Lizenzhinweis im Dokument

### Vorbereitung

Meine Vorbereitung für einen Kurs:

* ein Browser und eine Anmeldung auf GitLab
* ein Thema für den Kurs/die Einheit
* ein paar Textschnipsel z.B. aus [Wikipedia](https://de.wikipedia.org/wiki/Wikipedia:Hauptseite)
* ein paar Bilder z.B. von [Wikimedia Commons](https://commons.wikimedia.org/wiki/Main_Page)


### Projekt klonen - ein Template verwenden

1. neues Projekt erstellen -> + -> New Project -> Import project -> Repo by URL
  * [Vorlage](https://gitlab.com/TIBHannover/oer/course-metadata-test.git) (link kopieren) und bei "Git repository URL" einfügen
  * Project name - sprechenden Namen vergeben
  * Project slug - den gleichen Text, aber Leerzeichen durch Bindestriche ersetzen und Umlaute ausschreiben
  * Public machen
  * CREATE PROJECT
1. Metadaten mit [Generator](https://tibhannover.gitlab.io/oer/course-metadata-gitlab-form/metadata-generator.html) erzeugen und kopieren
1. Metadaten in metadata.yml einfügen
1. course.md bearbeiten mit [Markdown](https://gitlab.com/axel-klinger/gitlab-for-documents/blob/master/gitlab-markdown.md)

Nach dem Speichern (Commit changes) dauert es beim ersten mal ca. 15min, bis die generierte Seite unter SETTINGS -> PAGES verfügbar ist (solange gibt es einen 404). Weitere Änderungen stehen i.d.R. nach <1min bereit.

1. Adressen der Ausgabedateien in README anpassen mit SETTINGS -> PAGES -> Your pages are served under
1. Seite aufrufen von README aus  

Und hier das ganze nochmal im Video ...

<iframe width="560" height="315" src="https://www.youtube.com/embed/byRVOPM7qeg" allowfullscreen="allowfullscreen"></iframe>

... und hier das Ergebnis ...

<iframe width="560" height="315" src="https://www.youtube.com/embed/UfC0IWy87AI" allowfullscreen="allowfullscreen"></iframe>


## Die Oberfläche von GitLab

Video zu

* alles einmal angeklickt
* nützliche Features auch für OER


## Zusammenarbeiten mit GitLab

Video zu

* Issues
* Merge-Requests
* Bearbeitungsrechte


## Effizienter offline arbeiten

Offline arbeiten hat einige Vorteile

* man hat immer eine vollständige Kopie auf seinem eigenen Rechner
* viele Text-Editoren haben mächtige Werkzeuge für die Bearbeitung von Markdown und anderen Dateien

[Video mit Atom mehr Komfort für die Arbeit mir GitLab und Markdown]()


Der Nachteil ist

* wenn man nicht sauber synchronisiert, kann das zu Konflikten führen - die sich mittlerweile aber auch schon recht gut (z.B. in Atom) lösen lassen

[Video Konflikt durch parallele Arbeit auf Server]

Grundsätzlich kann jeder Editor für die Bearbeitung von Markdown verwendet werden. Im folgenden wird ein mögliches Szenario anhand des Editors Atom von https://atom.io gezeigt.

### Atom

Der Editor bietet eine gute Unterstützung von Markdown, erweiterbar durch einige Plaugins, und eine gute Anbindung an GitHub/GitLab.

Installation

* Git installieren von https://git-scm.com/downloads
* Atom installieren von https://atom.io

Ein paar Tastenkombinationen vorab

| Funktion                         | Windows       | Linux | Mac |
| -------------------------------- | ------------- | ----- | --- |
| Projekt klonen                   | ALT+G SHIFT+0 |       |     |
| Projektstruktur ein/ausblenden   | STRG+K STRG+B |       |     |
| Git-Ansicht ein/ausblenden       | STRG+SHIFT+9  |       |     |
| Vollbildanzeige                  | F11           |       |     |
| Markdown Preview ein/ausschalten | STRG+SHIFT+M  |       |     |

Tastenkombinationen können auch individuell angepasst werden über File -> Settings -> Keybindings und den Aufruf der Datei "your keymap file".


## ANHANG


## Welche Formate haben die Texte?

* **Eingabe :** Unformatierte Texte in [Markdown](gitlab-markdown.md). Später für Fortgeschrittene auch asciidoc oder LaTeX.

* **Ausgabe :** HTML, PDF, EPUB ... und alles was [Pandoc](https://pandoc.org/) unterstützt!


### Warum Versionskontrolle für Texte

Als Beispiel nehmen wir eine Studienarbeit mit ca. 50 Seiten, die in Word - inklusive der Bilder - eine Größe von etwa 10 MB hat. Jedes Mal, wenn wir sie unter einer neuen Version speichern, kommen weitere 10+ MB hinzu, auch wenn nur wenig geändert wurde.

Die gleiche Datei (das GitLab Projekt) hat in diesem Fall in Markdown eine Größe ca. 3 MB, da der größte Teil in Word die Microsoft eigenen Tags im Dokument sind und hier nur der reine Inhalt gespeichert wird. Wenn wir in GitLab eine Änderung einfügen, wird hier nur die Änderung mit wenigen KB als Version gespeichert. Es werden nicht alle enthaltenen Bilder und das ganze Dokument jedes mal wieder neu gespeichert.    

Weitere Vorteile sind u.a.

* mit Markdown: Trennung von Inhalt und Layout unterstützt die Nachnutzbarkeit
* detaillierte Historie der Änderungen


### Das Format Markdown

[Übersicht der Elemente](gitlab-markdown.md)


### Effizienter offline arbeiten

* Am Beispiel Atom (andere Editoren mit guter Markdown Unterstützung und Git-Anbindung sind ebenso möglich, wie z.B. Visual Studio Code oder auch diverse Apps für GitHub/GitLab)

[Video zur Offline-Arbeit mit Atom]()

### Konflikte Lösen!

> TODO !!!

### Grundlagen von Git

* Installation

#### Die Elemente

* Repository
* Working Direktory
* Commit
* Index
* Branch

#### Die Funktionen

Die folgende Auflistung bekommt man mit dem Aufruf von `git` ohne Parameter

```
start a working area (see also: git help tutorial)
   clone      Clone a repository into a new directory
   init       Create an empty Git repository or reinitialize an existing one

work on the current change (see also: git help everyday)
   add        Add file contents to the index
   mv         Move or rename a file, a directory, or a symlink
   reset      Reset current HEAD to the specified state
   rm         Remove files from the working tree and from the index

examine the history and state (see also: git help revisions)
   bisect     Use binary search to find the commit that introduced a bug
   grep       Print lines matching a pattern
   log        Show commit logs
   show       Show various types of objects
   status     Show the working tree status

grow, mark and tweak your common history
   branch     List, create, or delete branches
   checkout   Switch branches or restore working tree files
   commit     Record changes to the repository
   diff       Show changes between commits, commit and working tree, etc
   merge      Join two or more development histories together
   rebase     Reapply commits on top of another base tip
   tag        Create, list, delete or verify a tag object signed with GPG

collaborate (see also: git help workflows)
   fetch      Download objects and refs from another repository
   pull       Fetch from and integrate with another repository or a local branch
   push       Update remote refs along with associated objects
```
