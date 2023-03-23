# Excel-Bewertungsbogen für Leistungsnachweise

Ein Excel-Rechner um Leistungsnachweise aller Art (Klassenarbeiten, Klausuren, Lernkontrollen, Hausaufgaben etc.) zu bewerten.

**Download:** [Bewertungsbogen_Leistungsnachweis.xlsx](https://github.com/margomius/bewertungsbogen-leistungsnachweis/raw/main/Bewertungsbogen_Leistungsnachweis.xlsx)

Ausgefüllte Beispiel-Datei: [Bewertungsbogen_Leistungsnachweis_Beispiel.xlsx](https://github.com/margomius/bewertungsbogen-leistungsnachweis/raw/main/Bewertungsbogen_Leistungsnachweis_Beispiel.xlsx)

## Beschreibung

Mit diesem Excel-Rechner werden sämtliche Berechnungen für die Bewertung eines Leistungsnachweises automatisch vorgenommen:
* Punkteverteilung für die Benotung ("Für X Punkte gibt es Note Y")
* Gesamtpunktzahl der Schülys
* Noten der Schülys als Dezimal (1,0 bis 6,0), Gewichtung (1+ bis 6) und Oberstufenpunkte (0 bis 15)
* Berechnung des Fehlerindexes inkl. Abzug von 0 - 2 Notenpunkten.
* Notenspiegel (1 bis 6) und Punktespiegel (0 bis 15)
* Notenverteilung und Punkteverteilung als Säulendiagramm
* Durchschnittliche Punktzahl zu jeder Aufgabe (in Dezimal und in Prozent)
* Durchschnittliche Gesamtpunktzahl der ganzen Klasse
* Durchschnittliche Gesamtnote der ganzen Klasse (als Note und als Notenpunkte)
    * Hier wird kein Durchschnitt aller Noten berechnet, da dies mathematisch nicht zulässig ist. Stattdessen wird anhand der durchschnittlichen Gesamtpunktzahl eine Note und Notenpunkte bestimmt.
* Anzahl der Schülys, die schlechter sind als Note 4 oder 5 Notenpunkte (als Zahl und in Prozent)

## Anleitung

### Vorbereitung

1. Füge die Klassenliste in die Spalten D und E ein
    * **Für hessische Lehrkräfte:** Kurslisten lassen sich wie folgt aus dem Schulportal kopieren & einfügen: Schulportal Hessen > "Lerngruppen" > [Ihre Lerngruppe] > "+ Mehr" > "CSV"
2. Trage in Zeile 36 für jede Aufgabe ein, wie viele Bewertungseinheiten/Punkte es maximal zu erreichen gibt
    * Wenn Aufgaben nicht die benötigt werden, können die entsprechenden Zellen einfach freigelassen werden
    * Wenn mehr als zehn Aufgaben benötigt werden, kannst du dir über die Grupperung (+) über Spalte Z zehn weitere Spalten für Aufgaben einblenden lassen

Der Excel-Rechner zählt nun die erreichbaren Bewertungseinheiten/Punkte aller Aufgaben zusammen und zeigt die Summe in Zelle BA an. Das ist die Gesamtpunktzahl, die es in dem Leistungsnachweis zu erzielen gibt.
In der Tabelle darunter, wird eine Punkteverteilung generiert, die abhängig von der erreichbaren Gesamtpunktzahl ist.

3. **Optional:** Passe die Prozente in der Spalte BD an, um die Punkteverteilung des Leistungsnachweises zu verändern. Dies geht auch nachträglich. Standardmäßig sind dort die [Prozentwerte](https://www.rv.hessenrecht.hessen.de/bshe/document/hevr-OSt_AbiVHEV8Anlage9a) der Oberstufen und Abiturverordnung (OAVO) aus Hessen hinterlegt.
4. **Optional:** Über die Gruppierung (+) über Spalte AG können Spalten zur Berechnung des Fehlerindexes eingeblendet werden. Auch hier werden die [Vorgaben der OAVO](https://www.rv.hessenrecht.hessen.de/bshe/document/hevr-OSt_AbiVHEV6Anlage9b) aus Hessen verwendet.
    * Ab dem Fehleriundex 3: 1 Punkt Abzug
    * Ab dem Fehlerindex 6: 2 Punkte Abzug

### Bewertung des Leistungsnachweises

* Jede Zeile steht nun für den Leistungsnachweis eines Schülys.
* Während der Leistungsnachweis bewertet wird, kann für jedes Schüly und für jede Aufgabe die erreichte Punktzahl in die entsprechende Zelle geschrieben werden.
* Sämtliche Berechnung werden sofort durchgeführt und die alle Einstellungen können jederzeit noch angepasst werden.
* Die Tabelle kann nach allen Spalten sortiert werden (z.B. Gesamtpunktzahl)

## Weitere Funktionen

* Die Gesamtpunkzahl der Schülys wird durch eine Farbskala von grün (höchste Punktzahl) bis rot (niedrigste Punktzahl hervorgehoben)
* Wenn mehr als 1/3 der Klasse schlechter ist als Note 4, wird der Notenspiegel rot gefärbt
* Wenn mehr als 1/2 der Klasse schlechter ist als 5 Notenpunkte, wird der Punktespiegel rot gefärbt
* Wenn ein Schüly bei einer Aufgabe die volle Punktzahl erreicht hat, dann wird die Punktzahl fett dargestellt.
* Wenn für ein Schüly bei einer Aufgabe aus Versehen mehr Punkte eingetragen werden, als es maximal zu erreichen gibt, dann wird die Punktzahl rot dargestellt.
* Auf einem weiteren Tabellenblatt gibt es eine einfache Tabelle aller Aufgaben inkl. der erreichbaren Bewertugnseinheiten/Punkte und dem Klassendurchschnitt als Zahl und in Prozent. Diese Übersicht kann z.B. inkl. dem Notenspiegel den Schülys zur Verfügung gestellt werden.

## Screenshots

### Liste mit Schülys und den jeweiligen Aufgaben
![image](https://github.com/margomius/bewertungsbogen-leistungsnachweis/blob/main/Screenshots/Screenshot_1.PNG?raw=true)

### Punkteverteilung, Notenspiegel etc.
![image](https://github.com/margomius/bewertungsbogen-leistungsnachweis/blob/main/Screenshots/Screenshot_2.PNG?raw=true)

## Versionsverlauf

* 1.2
    * Anzahl der Aufgaben wurden wurde auf 20 erhöht
    * Aufgaben 11-20 wurden gruppiert
    * Fehlerindex wurde gruppiert
    * kleinere Updates und Fehlerbehebungen
* 1.1
    * Fehlerindex wurde hinzugefügt
    * kleinere Updates und Fehlerbehebungen
* 1.0
    * Initial Release 