# BlokBa

**Hybride blockbasierte Programmierung für den Unterricht.**

Schülerinnen und Schüler setzen Blöcke zusammen und sehen, wie diese **live in
echten Python-Code übersetzt** werden, der sofort ausgeführt wird. Der Code
steht Zeile für Zeile neben den Blöcken. Funktioniert vollständig offline.

Entwickelt für die Sekundarstufe I (11–15 Jahre) als Brücke zum eigenhändigen
Schreiben von Python.

> [Bosanski](README.md) · [English](README.en.md) · **Deutsch**

<!-- BILD: hier Screenshot des Hauptfensters einfügen -->

---

## Download

Neueste Version: **[Releases](../../releases/latest)**

| System | Download | Hinweis |
|---|---|---|
| Windows 10/11 | **[BlokBa.1.0.0.-portable.exe](https://github.com/DinoIsanovic/BlokBa-app/releases/download/BlokBa/BlokBa.1.0.0.-portable.exe)** | Keine Installation — einfach starten |
| Linux (64-Bit) | **[BlokBa-1.0.0.AppImage](https://github.com/DinoIsanovic/BlokBa-app/releases/download/BlokBa/BlokBa-1.0.0.AppImage)** | Eine Datei, keine Installation |

---

## Erster Start

### Windows

Beim ersten Start zeigt Windows ein blaues Fenster:

> **Der Computer wurde durch Windows geschützt**

**Das ist kein Virus.** Diese Meldung erscheint bei jedem Programm ohne
digitale Signatur. Eine Signatur kostet mehrere hundert Euro pro Jahr — für
eine kostenlose Schulanwendung schwer zu rechtfertigen.

Auf **Weitere Informationen** klicken, dann auf **Trotzdem ausführen**.

Python wird **nicht benötigt** — es ist im Programm enthalten.

### Linux

Die heruntergeladene Datei hat keine Ausführungsrechte. Im Terminal:

```bash
chmod +x BlokBa-1.0.0.AppImage
./BlokBa-1.0.0.AppImage
```

Oder Rechtsklick → *Eigenschaften* → *Zugriffsrechte* → *Ausführbar*.

**Python 3.10 oder neuer muss installiert sein.** Die meisten Distributionen
bringen es bereits mit. Falls nicht, meldet BlokBa das und zeigt den passenden
Installationsbefehl für das jeweilige System an.

---

<img width="1742" height="1034" alt="image" src="https://github.com/user-attachments/assets/1344fb2a-4452-413e-afc2-8acbdc1c9ec2" />


## Was BlokBa kann

- **11 Blockkategorien** — Start, Variablen, Ein-/Ausgabe, Mathematik,
  Bedingungen, Schleifen, Text, Listen, Zeichnen, Klang, Funktionen
- **Live-Python-Code** neben den Blöcken, damit sichtbar wird, was jeder Block
  bedeutet
- **Variablentabelle**, die sich während des Programmlaufs aktualisiert,
  inklusive Datentypen
- **Roboter-Assistent**, der Fehler in verständlicher Sprache erklärt — ohne
  Internet
- **Turtle-Grafik** auf einem Koordinatenraster
- **Export nach `.py`** — das Programm lässt sich in PyCharm öffnen und verhält
  sich identisch
- **Fünf Oberflächensprachen:** Bosnisch, Kroatisch, Englisch, Deutsch,
  Kyrillisch

---

## BoT — der Lernassistent

BlokBa bringt einen Assistenten mit, der auf **zwei Ebenen** arbeitet.

### Offline — immer verfügbar

Stürzt ein Programm ab, übersetzt BoT die Python-Fehlermeldung in verständliche
Sprache: was passiert ist, in welcher Zeile, und wie es sich beheben lässt.
Auch Endlosschleifen werden erkannt und erklärt.

Dafür wird **nichts benötigt** — kein Internet, kein Schlüssel, keine
Einrichtung. So funktioniert BlokBa im Klassenzimmer ohne Netz.

### Mit einem echten KI-Modell — optional

Wer möchte, dass Lernende in eigenen Worten fragen können, kann BoT mit einem
Sprachmodell verbinden:

| Dienst | Voraussetzung |
|---|---|
| Anthropic (Claude) | API-Schlüssel, Internet |
| OpenAI (GPT) | API-Schlüssel, Internet |
| Google (Gemini) | API-Schlüssel, Internet |
| **Ollama** | lokal installiertes Modell, **kein Internet** |

Einzurichten unter **AI Asistent → Postavi API ključ**. Der Schlüssel wird
**nur auf diesem Rechner** gespeichert und ausschließlich an den gewählten
Dienst gesendet.

BoT kennt die in BlokBa vorhandenen Blöcke und nennt sie beim Namen, statt
Python-Code vorzuschlagen, der sich mit Blöcken gar nicht bauen lässt. Die
Aufgabe wird nicht gelöst — es wird Schritt für Schritt hingeführt.

### Vor dem Einschalten

**Kosten.** Anthropic, OpenAI und Google rechnen nutzungsabhängig über das
eigene Konto ab. Google bietet ein kostenloses Kontingent, das zum Ausprobieren
in der Regel ausreicht.

**Datenschutz.** Bei einem Online-Dienst werden die Fragen und der Code der
Lernenden an diesen Anbieter übertragen. In der Arbeit mit Kindern verdient das
eine bewusste Entscheidung und einen Blick in die Richtlinien der Schule.
**Ollama behält alles auf dem Rechner** — nichts verlässt ihn.

**Ollama braucht einen leistungsfähigen Rechner.** Ein brauchbares Modell
belegt mehrere Gigabyte Arbeitsspeicher, idealerweise auf der Grafikkarte. Auf
älteren Schulrechnern ist das nicht realistisch — dort greift der
Offline-Assistent.

Der Online-Assistent bleibt **ausgeschaltet, bis er aktiviert wird.**

---

## Fehler melden und Vorschläge

<!-- LINK: hier Link zum Discord-Kanal einfügen -->

Bitte **immer die Versionsnummer angeben** (*Pomoć → O programu*) sowie das
Betriebssystem. Ohne diese Angaben lässt sich nicht feststellen, ob der Fehler
bereits behoben ist.

Ein Screenshot hilft mehr als eine Beschreibung.

---

## Das Projekt unterstützen

BlokBa ist kostenlos und bleibt es. Wer die weitere Arbeit unterstützen möchte:

Paypal: nodi_bih@yahoo.de

---

## Nutzungsbedingungen

BlokBa darf **kostenlos genutzt und in unveränderter Form weitergegeben**
werden — in der Schule und zu Hause.

Das Verändern, Umpacken und Verbreiten veränderter Versionen ist nicht
gestattet.

---

## Autoren

Dino Isanović · Jasmin Suljkanović · Elvir Čajić
