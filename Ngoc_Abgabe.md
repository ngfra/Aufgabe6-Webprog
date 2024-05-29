### Test Webprogrammierung 29.05.2024

**Name:**

**Anweisungen:** Beantworten Sie alle Fragen sorgfältig und vollständig. Die maximale Punktzahl für diesen Test beträgt 130 Punkte.

---

#### Teil 1: Planung eines Webprojektes (Relaunch)

**1.1.** Welchen wesentlichen Unterschied gibt es zwischen dem Relaunch einer bestehenden Webseite und der Planung einer neuen Webseite? (5 Punkte)

Antwort: Der Unterschiede sind, bei der Planung einer neuen Webseite muss man alles neu anfangen. Bei dem Relaunch muss man überlegen, welche Resourcen hat man schon, welche Verbeserrung, was kommt neues,...



**1.2** Beschreiben Sie die wesentlichen Schritte bei der Planung eines Website-Relaunchs. (10 Punkte)

Anwort:
  - Bestehende Website analysieren
  - Ziel und Zielgruppe definieren
  - Moodboard
  - Konzeption
  - Wireframes, Screendesign
  - Zwischen Präsentation, Feedback
  - Umsetzung
  - Online Stellung, Test



**1.3** Warum ist es wichtig, eine Bestandsaufnahme der aktuellen Website durchzuführen? Nennen Sie zwei Gründe. (5 Punkte)

Anwort:
- Welche Zustand, Probleme, Schwachstelle hat die Website, was muss verbessert werden,... (Responsive, SEO,...)
- Ob man die aktuelle Resourcen (Bilder, Text,..) wieder benutzen kann.

**1.4** Welche Rolle spielt die Zielgruppenanalyse bei einem Website-Relaunch? (5 Punkte)


- Die Zielgruppe noch einmal kennenlernen oder hat die Website neue Zielgruppe. Hilft bei dem Design der Website, ob es Mobile optimierung, oder hoch Kontrast,...
---

#### Teil 2: Git und Github

**2.1** Erklären Sie, was Git ist und wofür es verwendet wird. (5 Punkte)

- Git ist ein Versionkontrolle-Programm, die für Entwickler geeignet ist. Damit kann man die ganze Veränderung von Quellcode verfolgen.

**2.2** Was ist Github und wie unterscheidet es sich von Git? (5 Punkte)

- Github ist webbasierte Onlinedienst, wo die Quellcode gespeichert wird. Unterschied ist, auf Github kann man neue Repo anlegen, Zusammen im Team durch Invite arbeiten...

**2.3** Erklären Sie jeden der folgenden Begriffe: (10 Punkte)

* Repository: ein Ort, wo alles Details (Code, Beschreibung...) gesammelt und gespeichert werden.
* Branch: in der Repository, kann man ein neues Branch erstellen und separat unhängig arbeiten.
* Commit: die lokale Veränderung wird makiert.
* Merge: alle Code in z.B einem Branch wird zusammen mit Main vereint.
* Pull: die aktuellen Stand im Server runterladen.
* Push: die Veränderungen im lokalen Speicher hochladen.
* Clone: eine Repo auf lokalen Rechner kopieren.
* Remote Repository / Origin: Verwaltung die andere Branch, wenn gibts.
* Fetch: aktuellisiert den Stand von lokalen Rechner, ob der gleichen Stand wie im Server hat.
* Konflikt: gibt wenn im Team alle gleichzeitig pushen, oder der lokale Rechner hat keinen gleichen Stand wie im Server und will trotzdem was pushen.

---

#### Teil 3: CSS-Variablen nutzen

**3.1** Was sind CSS-Variablen und warum sind sie nützlich? (5 Punkte)

- CSS-Variablen sind die benutzer definierte CSS Eingeschaften. Die CSS Werte werden nur einmal geschrieben und kann man immer wieder benutzen. Man muss nur einmal verändern und es gilt auf die ganze Website.

**3.2** Überarbeite den folgenden CSS-Code, indem du redundante Werte identifizierst und entscheidest, welche in CSS-Variablen ausgelagert werden sollten. Achte auf sinnvolle Variablennamen. (10 Punkte)

```css

/* Farben */
/* Variable */
:root {
  --BgColor: #f0f0f0;
  --TextColor:#fff;
  --BgColor--btn:#007bff;
  --fontMain: Arial, sans-serif;
}


body {
  background-color: var(--BgColor);
}

.header {
  background-color: #333;
  color: var(--TextColor);
}

.button {
  background-color: #007bff;
  color: var(--TextColor);
  border: none;
  border-radius: 5px;
  padding: 10px 20px;
  cursor: pointer;
}

.card {
  background-color: var(--BgColor);
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
  border-radius: 10px;
  padding: 20px;
}

/* Schriftarten */
h1 {
  font-family: --fontMain;
}

p {
  font-family: --fontMain;
}

/* Abstände */
.container {
  margin: 20px;
}

.header {
  padding: 20px;
}

.card {
  margin-bottom: 20px;
}

/* Größen */
.button {
  font-size: 16px;
}

.card {
  width: 300px;
}

```

---

#### Teil 4: Komponentenbasierte Elemente für Websites entwickeln

**4.1** Was versteht man unter komponentenbasiertem Webdesign? (5 Punkte)

- komponentenbasiertem Webdesign benutzt die unabhängige Komponenten. Das heißt, die Komponenenten werden immer wieder verwendet für alle Seiten. Die funktionieren unabhängig.

**4.2** Nennen Sie zwei Vorteile der Nutzung von komponentenbasierten Elementen. (5 Punkte)

- Zeit sparen, man kann die Komponenten auf alle Seite verwendet, und Css nur einmal schreiben.
- Übersichtlicher, man weiß genau, welche Komponent auf welche Position.

**4.3** Erstellen Sie ein einfaches Beispiel für eine komponentenbasierte HTML-Struktur (Kartenkomponente mit Bild, Titel, Text). (10 Punkte)

```html
<!-- Beispiel HTML-Struktur für eine Kartenkomponente -->
<div class="cardImg">
  <div class="cardImg__image">
    <img src="" titel="" alt="">
  </div>
  <div class="cardImg__titel">
    <h3>Image Titel</h3>
  </div>
  <div class="cardImg__text">
    <p>Oh hell yeah I have a test!</p>
  </div>
</div>
```

---

#### Teil 5: Container Queries

**5.1** Was sind Container Queries und wie unterscheiden sie sich von Media Queries? (5 Punkte)

- Container Queries sind CSS Technik, eine neue Möglichkeit, Website responsive zu gestalten.
- Unterschied von Media Queries bezieht sich Container Queries nicht auf die gesamte Breite des Viewports sondern auf die Breite der Container.

**5.2** Beschreiben Sie eine Situation, in der Container Queries besonders nützlich sein können. (5 Punkte)

- Bei dem Design mit display grid, wo die Element dynamisch plaziert werden, es ist nützlich Container Queries zu benuten.

**5.3** Erweitern Sie den folgenden **CSS-Code** um eine Container Query, sodass der Innenabstand eines Elements bis zu einer Containerbreite von 400px (width) 20px beträgt. (10 Punkte)

```css

.container {

}

.box {
  padding: 40px;
}

/* Container Query */
@container (max-width:400px) {
  .box {
    paddind: 20px;
  }
}

```


```html
<div class="container">
  <div class="box">
    Dies ist eine Beispiel-Box mit variabler Schriftgröße.
  </div>
</div>
```

---

#### Teil 6: Praktische Aufgabe

Sie erhalten ein bestehendes Webprojekt auf Github und sollen einen Relaunch planen und teilweise umsetzen. Gehen Sie wie folgt vor: (30 Punkte)

0. Erstellen Sie ein Repository "Aufgabe6-Webprog" auf Ihren lokalen Rechner und kopieren Sie den Inhalt aus dem Ordner "Daten" hinein.
1. Erstellen Sie den "initial commit"
2. Erstellen Sie einen neuen Branch mit dem Namen "relaunch".
3. **Durchführen der folgenden Änderungen:**
   - **CSS-Variablen:** Definieren Sie sinnvolle CSS-Variablen und verwenden Sie diese in Ihrer CSS-Datei.
   - **Komponentenbasierte Elemente:** Entwickeln Sie eine einfache, komponentenbasierte HTML-Struktur für eine Kartenkomponente, die einen Titel, ein Bild und einen Text enthält.
   - **Container Queries:** Implementieren Sie eine Container Query, um die Schriftgröße der Kartenkomponente basierend auf der Containergröße anzupassen. Verwenden Sie eine Schriftgröße von 1rem bis zu einer Containerbreite von 540px.
4. **Committen Sie Ihre Änderungen:** Geben Sie nach jedem bedeutenden Schritt einen aussagekräftigen Commit-Namen an und committen Sie Ihre Änderungen.
5. **Merge:** Führen Sie einen Merge des "relaunch"-Branches zurück in den Haupt-Branch ("main") durch.
6. Erstellen Sie auf ihrem Github-Account ein neues öffentliches Repository mit dem Namen "Abgabe-Webprog".
7. Notieren Sie hier die URL zu Ihrem Repo auf Github: https://github.com/ngfra/Aufgabe6-Webprog
8. Pushen Sie Ihr lokales Repository in das neu erstellte Remote-Repository.
9. Speichern Sie zusätzlich alle lokalen Dateien als ZIP-Datei "vorname-nachname.zip" und mailen diese an manuel@startmedia.at