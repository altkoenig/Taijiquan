# GitHub, GitHub Desktop und Visual Studio Code einrichten

Eine Schritt-für-Schritt-Anleitung für Windows, ohne Vorkenntnisse.

---

## Worum geht es?

| Was | Wofür | Muss man installieren? |
|---|---|---|
| **GitHub** | Eine Webseite, auf der deine Dateien sicher online gespeichert und mit anderen geteilt werden. Stell es dir wie einen Cloud-Ordner vor, der sich jede Änderung merkt. | Nein, du legst nur ein kostenloses **Konto** an. |
| **GitHub Desktop** | Ein Programm auf deinem PC, das deine Dateien mit GitHub abgleicht, per Mausklick. | Ja |
| **Visual Studio Code** (kurz „VS Code“) | Ein Programm zum Bearbeiten von Texten und Dateien (z. B. diese `.md`-Datei). | Ja |

Geh am besten in genau dieser Reihenfolge vor: **1. Konto → 2. GitHub Desktop → 3. VS Code.**

---

## Schritt 1: GitHub-Konto anlegen

1. Öffne im Browser die Seite **<https://github.com>**
2. Klick oben rechts auf **„Sign up“** (Registrieren).
3. Gib ein:
   - deine **E-Mail-Adresse**
   - ein **Passwort** (mindestens 15 Zeichen, oder mindestens 8 Zeichen mit einer Zahl und einem Kleinbuchstaben)
   - einen **Benutzernamen** (der ist später öffentlich sichtbar, z. B. `maxmustermann`)
4. Löse das kleine Rätsel, das prüft, ob du ein Mensch bist.
5. GitHub schickt dir einen **Code per E-Mail**. Schau in dein Postfach (ggf. auch im Spam-Ordner) und tipp den Code auf der Webseite ein.
6. Fragen nach Team-Größe, Interessen usw. kannst du überspringen („Skip“). Wähl den **kostenlosen Tarif (Free)**.

✅ Fertig: Du hast jetzt ein GitHub-Konto. Notier dir Benutzername und Passwort.

> **Tipp:** GitHub verlangt meist die **Zwei-Faktor-Anmeldung** (2FA). Dafür brauchst du eine App auf dem Handy, z. B. *Microsoft Authenticator* oder *Google Authenticator*. GitHub führt dich durch die Einrichtung. Die angezeigten **Wiederherstellungscodes** (Recovery Codes) unbedingt ausdrucken oder sicher speichern!

---

## Schritt 2: GitHub Desktop installieren

1. Öffne **<https://desktop.github.com>**
2. Klick auf **„Download for Windows“**.
3. Öffne die heruntergeladene Datei (meist im Ordner **Downloads**, Name z. B. `GitHubDesktopSetup-x64.exe`) per Doppelklick.
4. Die Installation läuft **automatisch** durch, du musst nichts auswählen. Danach öffnet sich GitHub Desktop von selbst.

### GitHub Desktop mit deinem Konto verbinden

1. Klick im Begrüßungsfenster auf **„Sign in to GitHub.com“**.
2. Es öffnet sich der Browser. Melde dich mit deinem GitHub-Konto an und klick auf **„Authorize desktop“** (Zugriff erlauben).
3. Der Browser fragt evtl., ob er „GitHub Desktop öffnen“ darf: mit **Ja / Öffnen** bestätigen.
4. Zurück in GitHub Desktop: Bei **„Configure Git“** sind Name und E-Mail meist schon eingetragen. Klick auf **„Finish“**.

✅ Fertig: GitHub Desktop ist eingerichtet.

> **Gut zu wissen:** GitHub Desktop bringt das Hilfsprogramm **Git** bereits mit. Du musst Git nicht extra installieren.

---

## Schritt 3: Visual Studio Code installieren

1. Öffne **<https://code.visualstudio.com>**
2. Klick auf den großen Button **„Download for Windows“**.
3. Öffne die heruntergeladene Datei (z. B. `VSCodeUserSetup-x64-....exe`) per Doppelklick.
4. Geh durch den Installations-Assistenten:
   - **Lizenzvereinbarung:** „Ich akzeptiere die Vereinbarung“ → **Weiter**
   - **Zielordner:** so lassen → **Weiter**
   - **Startmenü-Ordner:** so lassen → **Weiter**
   - **Zusätzliche Aufgaben:** Hier am besten **alle Häkchen setzen**, besonders:
     - ☑ *Desktopsymbol erstellen*
     - ☑ *Aktion „Mit Code öffnen“ dem Dateikontextmenü hinzufügen*
     - ☑ *Aktion „Mit Code öffnen“ dem Verzeichniskontextmenü hinzufügen*
     - ☑ *Zu PATH hinzufügen* (sollte schon angehakt sein)
   - → **Weiter** → **Installieren** → **Fertigstellen**

### VS Code auf Deutsch umstellen (optional)

1. Öffne VS Code.
2. Unten rechts erscheint oft der Hinweis *„Install language pack to change the display language to German“*. Klick auf **„Install and Restart“**. Fertig.
3. Falls der Hinweis nicht erscheint: Drück **Strg + Umschalt + X**, gib im Suchfeld **„German“** ein, klick beim Eintrag *„German Language Pack for Visual Studio Code“* auf **Install** und starte VS Code neu.

✅ Fertig: VS Code ist installiert.

---

## Schritt 4: GitHub Desktop und VS Code verbinden

Damit GitHub Desktop deine Dateien direkt in VS Code öffnen kann:

1. In GitHub Desktop oben im Menü: **File → Options** (Datei → Optionen).
2. Klick links auf **„Integrations“**.
3. Wähl bei **„External Editor“** den Eintrag **„Visual Studio Code“** aus.
4. Mit **„Save“** speichern.

---

## Schritt 5: Ein Projekt (Repository) auf den PC holen

Ein **Repository** (kurz „Repo“) ist einfach ein Projektordner, den GitHub verwaltet.

1. In GitHub Desktop: **File → Clone repository…** (Datei → Repository klonen).
2. Im Reiter **„GitHub.com“** siehst du deine Projekte und die, zu denen du eingeladen wurdest. Klick das gewünschte an.
   (Alternativ kannst du im Reiter **„URL“** die Internetadresse des Projekts einfügen.)
3. Unten bei **„Local path“** steht, wo der Ordner auf deinem PC landet, üblicherweise
   `C:\Users\<DeinName>\Documents\GitHub\<Projektname>`
4. Klick auf **„Clone“**.
5. Danach auf **„Open in Visual Studio Code“** klicken, und schon kannst du die Dateien bearbeiten.

---

## Der tägliche Ablauf: Änderungen speichern und hochladen

So bringst du deine Änderungen von deinem PC zu GitHub:

1. **Bearbeiten:** Datei in VS Code ändern und speichern (**Strg + S**).
2. **Zu GitHub Desktop wechseln:** Links unter **„Changes“** siehst du, welche Dateien du geändert hast. Grün = neu hinzugefügt, Rot = entfernt.
3. **Beschreiben:** Trag unten links im Feld **„Summary“** kurz ein, was du geändert hast, z. B. *„Kapitel 3 ergänzt“*.
4. **Festhalten:** Klick auf den blauen Button **„Commit to main“**. Damit ist die Änderung *auf deinem PC* gespeichert.
5. **Hochladen:** Klick oben auf **„Push origin“**. Jetzt ist die Änderung *auf GitHub* und für andere sichtbar.

Und umgekehrt, um Änderungen von anderen zu holen:

- Klick oben auf **„Fetch origin“**. Gibt es Neues, wird daraus **„Pull origin“**: noch einmal klicken.

> **Merksatz:** Vor dem Arbeiten **Pull**, nach dem Arbeiten **Commit + Push**.

---

## Kleines Wörterbuch

| Begriff | Bedeutung |
|---|---|
| **Repository / Repo** | Projektordner, den GitHub verwaltet |
| **Clone** | Ein Repo von GitHub auf den eigenen PC kopieren (macht man nur einmal) |
| **Commit** | Einen Zwischenstand mit kurzer Beschreibung festhalten |
| **Push** | Festgehaltene Änderungen zu GitHub hochladen |
| **Fetch / Pull** | Neue Änderungen von GitHub abholen |
| **main** | Der Hauptzweig, also die „offizielle“ Version des Projekts |
| **.md-Datei** | Textdatei im *Markdown*-Format: einfacher Text mit Zeichen wie `#` für Überschriften oder `**fett**` |

---

## Wenn etwas nicht klappt

- **Download startet nicht / Windows warnt:** Prüf, ob du wirklich auf den offiziellen Seiten bist (`github.com`, `desktop.github.com`, `code.visualstudio.com`). Bei der Windows-Warnung „Der Computer wurde durch Windows geschützt“ klickst du auf **„Weitere Informationen“ → „Trotzdem ausführen“**, aber nur bei Dateien von diesen Seiten.
- **Anmeldung in GitHub Desktop klappt nicht:** In GitHub Desktop **File → Options → Accounts** → **Sign out** und neu anmelden.
- **„Push“ wird abgelehnt:** Meist hat jemand anderes inzwischen etwas geändert. Klick erst auf **„Pull origin“**, dann erneut auf **„Push origin“**.
- **VS Code zeigt Markdown nur als Text:** Mit **Strg + Umschalt + V** öffnet sich eine schön formatierte Vorschau.
