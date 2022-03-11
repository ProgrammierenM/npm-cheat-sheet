# Node Package Manager Tutorial

Der Node Package Manager ist ein Tool mit dem du ganz bequem javaScript Pakete/Module für deine Projekte verwalten kannst. Ich zeige dir in diesem NPM Tutorial wie du Pakete installieren, updaten, löschen und anzeigen kannst.

Ich zeige dir die package.json Datei im Detail und was die einzelnen Versionsnummern bedeutet. Wir versionieren auch das eigene Projekt mit NPM und erstellen auch Script Befehle welche automatisch dein Projekt versionieren und mit GIT ein neuer Commit gemacht wird. Happy Coding

[Tutorial auf YouTube anschauen](https://youtu.be/Hb24A6VGYZ0)

[![Tutorial bei Youtube](http://img.youtube.com/vi/Hb24A6VGYZ0/0.jpg)](https://youtu.be/Hb24A6VGYZ0)

## Vernetze dich:

[<img align="left" alt="programmierenmitmario.de" width="22px" src="https://raw.githubusercontent.com/iconic/open-iconic/master/svg/globe.svg" />][website]
[<img align="left" alt="programmierenmitmario | YouTube" width="22px" src="https://cdn.jsdelivr.net/npm/simple-icons@v3/icons/youtube.svg" />][youtube]
[<img align="left" alt="programmierenmitmario | Twitter" width="22px" src="https://cdn.jsdelivr.net/npm/simple-icons@v3/icons/twitter.svg" />][twitter]
[<img align="left" alt="programmierenmitmario | Instagram" width="22px" src="https://cdn.jsdelivr.net/npm/simple-icons@v3/icons/instagram.svg" />][instagram]
<br>
<br>

## NPM Cheat Sheet

### Projekt initialisieren

<pre>
npm init
</pre>

### Projekt initialisieren (mit Defaultwerten)

<pre>
npm init -y
</pre>

### Defaultwerte ändern

<pre>
// Beispiele
npm config set init.license MIT
npm config set init.author.name "Max Mustermann"
npm config set init.author.email max@email.com
</pre>

### Defaultwerte anschauen

<pre>
// Beispiele
npm config get init.license
npm config get init.author.name
</pre>

### Defaultwerte löschen/reset

<pre>
// Beispiele
npm config delete init.license
npm config delete init.author.name
</pre>

## Pakete verwalten

### Pakete installieren

<pre>
// Das Paket express für das Projekt installieren
npm install express

// Nodemon als devDependency installieren
npm install -D nodemon

// Nodemon global installieren
npm install -g nodemon
</pre>

### Pakete aktualisieren

<pre>
// einzelenes Paket aktualisieren
npm update express

// Alle pakete aktualisieren
npm update
</pre>

### Pakete löschen

<pre>
// Beispiel
npm remove nodemon
</pre>

### installierte Pakete anzeigen

<pre>
// Alle Pakete anzeigen
npm list

// Anzeige minimieren
npm list --depth=0

// Ein spezielles Paket anzeigen
npm list jquery

// Global installierte Pakete anzeigen
npm list -g
</pre>

### Anzeigen welche Pakete veraltet sind

<pre>
npm outdated
</pre>

## Projektversionierung

### Versionsnummer erhöhen

1.0.0
(Major.Minor.Patch)

<pre>
// Patch (1.0.1)
npm version patch

// Minor (1.1.0)
npm version minor

// Major (2.0.0)
npm version major
</pre>

### Version erhöhen ohne das bei GIT ein Tag erstellt wird

<pre>
npm version patch --no-git-tag-version
</pre>

## License

[MIT](LICENSE)

[website]: http://programmierenmitmario.de
[twitter]: https://twitter.com/programmierenm
[youtube]: https://youtube.com/programmierenmitmario
[instagram]: https://instagram.com/programmierenm
