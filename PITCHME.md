###### Methoden der Softwareentwicklung

## Programmablaufpläne (flowcharts)

---

## Algorithmen

+++

### Abgrenzung



- Methoden der Softwareentwicklung
  - Algorithmen entwerfen
  - Fehler finden
- Algorithmen und Datenstrukturen
  - Algorithmen beurteilen (Speicherplatzbedarf, Geschwindigkeit, ...)
  - Alogrithmen verbessern
- C
  - Algorithmen implementieren

+++

### Definition

Ein _Algorithmus_ ist eine _eindeutige Handlungsvorschrift_ zur Lösung eines Problems. Algorithmen bestehen aus _endlich vielen_, _wohldefinierten Einzelschritten_.  
Damit können sie zur Ausführung in einem Computerprogramm implementiert, aber auch in menschlicher Sprache formuliert werden. Bei der Problemlösung wird eine bestimmte Eingabe in eine bestimmte Ausgabe überführt.

+++

### Eigenschaften

1. Endlichkeit (Finitheit)
2. Terminiertheit
3. Determiniertheit
4. Determinismus
5. Effizienz

+++

### Keine Unendlichkeit

- Endlichkeit (Finitheit), siehe auch [Komplexität](https://de.wikipedia.org/wiki/Komplexität_%28Informatik%29)
  - Statisch: Der Algorithmus hat endlich viele Schritte
  - Dynamisch: Der Algorithmus läuft mit endlich viel Prozessor- und Speicherkapazität

- Terminiertheit
  - Der Algorithmus endet für jede Eingabe

+++

### Deter... - was?!?

- [Determiniertheit](https://de.wikipedia.org/wiki/Determiniertheit_%28Algorithmus%29):
  - Bei gleicher Eingabe liefert der Algorithmus immer die gleiche Ausgabe

- [Determinismus](https://de.wikipedia.org/wiki/Determinismus_%28Algorithmus%29):
  - Bei gleicher Eingabe durchläuft der Algorithmus immer die gleiche Folge von Schritten
  - Deterministische Algorithmen sind immer auch determiniert

+++

### Und was noch?

- Effektivität:
  - Der Effekt jeden Schrittes ist eindeutig festgelegt

+++

## Wie findet man einen Algorithmus?

„Übung macht den Meister“

+++

### Übung


Formuliere Algorithmen in natürlicher Sprache

- Ein Bad nehmen
- Aufbackpizza backen
- Straße überqueren

---

## Programmablaufpläne

+++

```javascript
//Dies ist ein Codeblock

var i;
i = 3;

```

+++

### Warum Algorithmen grafisch darstellen?

- "Ein Bild sagt mehr als tausend Worte"  
  Bilder sind intuitiv leichter erfassbar als Quellcode

- Programmablaufpläne sind daher gut geeignet zur
  - Übersicht
  - Dokumentation
  - Kommunikation

+++

### Definition

> Ein _Programmablaufplan_ (PAP) ist ein Ablaufdiagramm für ein Computerprogramm, das auch als Flussdiagramm (engl. flowchart) oder Programmstrukturplan bezeichnet wird.  
> Es ist eine graphische Darstellung zur Umsetzung eines Algorithmus in einem Programm und beschreibt die Folge von Operationen zur Lösung einer Aufgabe.

+++

### Eigenschaften

- Leicht lesbar

- Zeigen die Struktur des Programms

- Verwenden wenige grafische Symbole für verschiedene Vorgänge

- Genormt in DIN 66001

+++?image=assets/images/papdef-startende.png&size=40%

### Start / Ende

- Kommen jeweils genau einmal vor

- Name nicht vergessen

+++?image=assets/images/papdef-eingabeausgabe.png&size=40%

### Eingaben / Ausgaben

- Können mehrfach vorkommen

- Eingaben typischerweise per Tastatur

- Ausgaben typischerweise per Monitor

- Wichtig: Eingaben einen Namen zuweisen 
  - Braucht ihr in Operationen
  - Gut: "Zahlen `a`, `b` und `c`" 
  - Schlecht: "3 Zahlen"

+++?image=assets/images/papdef-operation.png&size=40%

### Operationen

- Zentrale Elemente im PAP

- Je ein Eingangs- und ein Ausgangspfeil

- Exakt definiert. Möglicher Inhalt:

  1. Variablendeklaration (Bsp: `int i`)
  2. Wertzuweisung (Bsp: `i = 3`)
  3. Beides gleichzeitig (Bsp: `int i = 3`)

+++?image=assets/images/papdef-kommentar.png&size=49%

### Kommentare

- Enthalten Zusatzinformation

- Tragen zum besseren Verständnis des Programms bei

- Erklären schwierige Sachverhalte

- Helfen bei der (Wieder-) Einarbeitung

- Können ToDos für die Weiterentwicklung enthalten

+++?image=assets/images/papdef-abfrage.png&size=40%

### Abfragen

- Ermöglichen unterschiedliche Reaktion auf Eingaben

- Verzweigen Programmfluss nach Wenn-Dann-Prinzip

- Exakt definiert. Enthaltene Ausdrücke müssen auf

  - Ja (`true` bzw. `1`) oder 
  - Nein (`false` bzw. `0`) auswerten  
    Bsp: `i == 10` oder `x < 5`

+++?image=assets/images/papdef-schleife.png&size=40%

### Schleifen

- Abbruchbedingung entweder im Kopf oder im Fuß
- Symbol ersetzt Abfrage mit Abbruchbedingung
- Kopfgesteuert: erst Abbruchbedingung testen
- Fußgesteuert: erst Schleifeninhalt ausführen

+++?image=assets/images/papdef-unterprogramm.png&size=40%

### Unterprogramme

- Sinnvoll wenn gleiche Programmteile mehrfach vorkommen
- Verringern die Redundanz (DRY)
- Erhöhen die Übersicht
- Werden so entworfen als stünde der Inhalt direkt im PAP
- Ggf: Parameter in Kommentar definieren

+++

### Übung 1

Erstelle einen Programmablaufplan, der das Maximum dreier Zahlen `a`, `b` und `c` ausgibt.

+++

### Übung 1 - Lösung A

<img src="assets/images/ex-maxdreizahlen-a.png" style="width: auto; height: 550px">

+++

### Übung 1 - Lösung B

<img src="assets/images/ex-maxdreizahlen-b.png" style="width: auto; height: 550px">
