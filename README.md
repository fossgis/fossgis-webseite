# FOSSGIS Webseite

Die FOSSGIS-Website wird aus den Inhalten, die in den untergeordneten Verzeichnissen existieren, erzeugt. Die Struktur der Website wird durch die Struktur in `content` definiert. So sind z.B. alle Nachrichtenartikel im Verzeichnis `content/news`.

Um einen neuen Newsartikel anzulegen, muss eine neue Datei in `content/news` mit der Endung `.md` (Markdown) angelegt werden. Ein Artikel beginnt mit den Metadaten ganz oben:

	---
	title: "Dies ist ein Titel"
	date: "2019-02-29T15:00:00+02:00"
	author: "Marta Musterfrau"
	---

Anschließend kann der Inhalt geschrieben werden, z.B.

```markdown
## Unterüberschrift

Hier ist etwas Text.

Und hier ist ein neuer Absatz.
```

Statische Inhalte wie Bilder und dergleichen, die nicht von Hugo interpretiert werden sollen, gehören unter `static`, nicht nach `content`.

Lokal kann die Webseite mithilfe von hugo generiert werden: [Hugo Installationsanweisungen](https://gohugo.io/getting-started/installing/). Anschließend kann im Verzeichnis `hugo serve` ausgeführt werden. Dies startet einen lokalen Webserver, der üblicherweise unter [http://localhost:1313](http://localhost:1313) zu erreichen ist.

Im Zweifelsfall Inhalte anlegen und Pull Request öffnen, wir finden eine Lösung :)

## Tipps für Inhalte

- Überschriften mit max. 80—100 Zeichen
- Die Dateinamen bestimmen die spätere URL, bitte kurz und prägnant, wie z.B. `fossgis-2019-cfp.md`
