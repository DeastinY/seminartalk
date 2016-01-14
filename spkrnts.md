# Speaker's notes

## TITELFOLIE
Motivation :
- Visualisierung wichtig
  - Schnell/überhaupt verstehen
  - Daten erforschen / Zusammenhänge
  - Auge schnell und effizient
  - Einfache Interpretation
  - Einmaliger Aufwand / Dauerhafter Nutzen
- Weiterer Schwerpunkt
  - Multidimensionale Daten
  - Komplexe Probleme
    - Vorhersagen
    - Messungen
    - Bachelorarbeit (Einflüsse auf Performance)
  - Optische Zusammenhänge erkennen
  - Komplexe Ergebnisse fassbar machen

-> Vorgehen in dieser Präsentation
## ROADMAP
- Gute Mult. Dim. Vis. = Gute Vis. + Mult. Dim. Vis.
- Allgemeines
  - Workflow von Rohdaten bis Vis.
  - Fallstricke die man Umgehen kann
    - und Konzepte um Vis. Gut zu machen
    - Dabei Allg. + Spezielles
- Spezielles
  - Passende Vis. für mehrdim. Daten
- Kombinieren
  - *Gute* Vis. Mult. Dim.

-> Beginn mit abstraktem Prozess um aus Daten Vis. zu machen.

## VISUALISIERUNGSPIPELINE
Zuerst einfach erklären, dann etwas "philosophisch  
Erklärung :
1. Daten(-gewinnung)
  - Aufzeichen, Berechnen, Auslesen -> Es gibt Daten als Grundlage
  - Ohne Daten keine Visualisierung
2. Filter(bereinigung)
  - Nicht gewünschte Daten (die auch gemessen wurden) entfernen
  - Eventuelle normalisierung, Ausreisser anpassen
    - Verfälschung, kann aber angebracht sein
3. Design (Konvertierung)
  - Passende Darstellung entwerfen
  - Daten und Zahlen zu Formen und Bildern
4. Darstellung (Implementierung)

Ein mögliches Modell, allerdings praktisch um Fehler zuzuordnen  
zum Beispiel:
- Vis. zeigt nicht den geplanten Zusammenhang
  - Filterung falsch
- Daten richtig aber Vis. verwirrend, Wirkung verfehlt
  - Design unzureichend
  - Evtl. stärker/besser Filtern
- (interaktive) Visualisierung langsam
  - Schlechte Implementierung

Allgemein:
- Modell um Ursachen zu finden
- Eventuell auf einige Schritte keinen Einfluss
  - Frameworks (Implementierung)
  - Daten bereits gemessen (Man kann nichts weiteres messen)
- Abstrakt aber dadurch universell
- sehr praktisch im "Alltag"

-> Vom allgemeinen zu spezielleren Fällen
-> Vom "Visualisierungsworkflow" zu "Häufigen Fehlern"
- Zuerst 2 in den Medien genutzte Elemente, die im wissenschaftlichen Bereich nichts verloren haben, dann 2 allgemeine Hilfen, "zuletzt erkläre ich, warum man Kreisdiagramme verbieten sollte"

## IRREFÜHRENDE SKALIERUNG
- Sender Fox News - 2012  
- Änderungen im Spitzensteuersatz.  
- Steuersatz Verfünffacht sich ! - Eigentlich anstieg von 4.6 %  
- Skalierung beginnt bei 34 %  
- Hier genutzt um dramatisch Wirken zu lassen  
- In Wissenschaft undenkbar

-> Immer auf korrekte Skalierung achten, Daten können schnell verfälscht werden : z.B. Zoom

## VERZERRUNG DURCH EFFEKTE
- Steve Jobs MacWorld 2008 (iPhone 1 Anfang des Jahres)
- 19.5% größer als 21.2% von Nokia
- 3D Effekt für 2D-Graph
- Verzerrt immer !
- Unnötig
- Kreisdiagramm auch nicht ideal -> später

-> Bei Effekten immer Acht geben !
-> Jetzt allgemeineres, wo auch Effektprobleme aufgegriffen werden

## CHARTJUNK
- Edward Tufte, Informationswissenschaftler und Grafikdesigner
- Kritik an Powerpoint "Powerpoint is evil"
  - Powerpoint mit Ursache für Absturz der Challenger (In Arbeit nachlesen)
  - (Kritik z.B. poor typography and layout, simplistic thinking: bulletpoionts)
- Chartjunk: nutzlose, informationslose oder informationsverdunklnde Bestandteile
- Bleibt vielleicht besser in Erinnerung, Daten aber kaum zu erkennen
- Daten schnell verfälscht (Proportionen)
- Wissenschaftlichen auf jeden Fall unangemessen,
- eventuell auch im allg. Falsch, aber das ist diskussionwürdig
- Mitnehmen kann man:
  - Jegliche dekorativen Elemente unterlassen
  - Tinte nur benutzen um Informationen darzustellen -> Data Ink Ratio

## DATA-INK RATIO
- Edward Tufte
- "Above all else: Show the data !" (Tufte 1983)
- Data-Ink : Tinte (Pixel) die Informationen darzustellen
- Verhältnis Data-Ink zu Style-Ink sollte maximiert werden
- Alle unnötigen Elemente weglassen
  - Hintergrund
  - Redundante Beschriftung
  - Rahmen
  - Hilfslinien (weg oder schwach)
  - Schrift abschwächen
  - Reduzierte Farben
  - ...

## KREISDIAGRAMME
## 1- UND 2-DIMENSIONAL
## 3-DIMENSIONAL
## N-DIMENSIONAL
### TABLE
### COMPRESSED TABLE
### SCATTERPLOT MATRIX
### PARALLEL COORDINATE MATRIX
## ZUSAMMENFASSUNG
