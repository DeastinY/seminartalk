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

-> Beginn mit Grundlagen der Visualisierung

## Grundlagen
- Ziel der Visualisierung : Wissen vermitteln
- Andere müssen Wissen nicht erarbeiten, sondern man zeigt Ergebnisse
- (Wissenschaftlich anders, aber Grundgedanke gleich)
- Wichtig sind
- Motivation:
  - Warum präsentieren ? Ziel ?
  - Wissenschaft: Präzise These !
  - Nur dann möglich:
    - Daten reduzieren
    - Nur Wichtiges präsentieren
- Zielgruppe:
  - Wer wird angesprochen ?
  - Kultur, Umfeld, Interessen, Wissen
  - Unterschied: Arbeit (Fachwissen), Öffentlich oder z.B. Kindergarten
  - Auch Alter (Ghostbusters 1 - 18 Jahre alt, Kasetten oder Schallplatten zunehmend unbekannt)
  - Oder Interessen: Fußballverein oder Startrek Fans

-> Damit alles so glatt läuft: Motivation und Zielgruppe immer klar
-> Nach Grundlagen jetzt detailiert die Erstellung einer Visualisierung

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

-> Bereits angekündigt, jetzt ein Fall gegen Kreisdiagramme

## KREISDIAGRAMME
- Grundsätzlich nicht falsch, aber
- Sehr oft falsch verwendet
- Daten (Steve Jobs) werden sehr leicht verfälscht
- Vergleich vieler (ähnlicher) Größen schwierig
- Beispiel: Balkendiagramme viel besser
- Meist sollten Kreisdiagramme nicht genutzt werden
  - Wenig Nutzen bei wenig Teilen (Text)
  - Kein Nutzen bei vielen Teilen (Balkendiagramm)
- Wenn doch benutzen dann nur:
  - Zwei oder Drei Teile eines Ganzen
  - Sehr Unterschiedliche Werte
- Im Allgemeinen:
  - Ersatz durch kleine Tabellen, Sätze und/oder andere Diagramme ist schnell gefunden

-> Genug gelernt um gute Visualisierung zu erstellen, jetzt mehrdimensionalität
-> Dazu Unterteilung erst 1/2 und 3 Dimensionales, dann n-Dimensionales

## 1- UND 2-DIMENSIONAL
- Eindimensional:
  - "Zahlenstrahl" zeigt einfache Datenverteilung
  - Relativ selten
- Zweidimensional:
  - Meisten bekannten Graphen sind Zweidimensional
  - Liniendiagramm (einfach, komplex) (Anzahl/Wert)
  - Balkendiagramm (hier: gestapelt, auch oft: gruppiert) (Anzahl Wert)
  - Streudiagramm (Jeder Punkt ein Datensatz (Höhe/Gewicht))
  - Kastengrafik (Box-Whisker-Plot), median, quartile, ausreißer, minima, maxima
    - (Zwischen zwei Quartilen (95 Quartil) liegen X % aller Werte)

Beispiele:
  - Zeit/Temperatur
  - Haushalte/Haustiere
  - Anzahl/Klausurnote

-> Ziemlich viele bekannte Darstellungsformen
-> Jetzt bereits weniger weit verbreitete Formen

## 3-DIMENSIONAL
- Drei Raumkoordinaten. Farbe genutzt um Höhe anzuzeigen
  - Farbe für andere Information (z.B. Temperatur) -> vierdimensional
- Streudiagramm, zeigt (hier gruppierte) Datensätze im Raum an
- Heatmap X und Y Wert wird über Farbwert Information zugeordnet (hier: Jahr, Monat, Temperatur)
- Karte mit Todesfällen zu Adressen Eingetragen (Seminarvortrag) Karte (2D) + Balken
- (John Snow, 1984, Broadstreet, Cholera Epedemie)

-> Jetzt n-dimensionales, meist nur im wissenschaftlichen Bereich zu finden

## N-DIMENSIONAL
- Alles mit mehr als drei Dimensionen
  - Raumkoordinaten + Temperatur
  - Spieler, Jahre an Erfahrung, Treffer insgesamt, Treffer im Durchschnitt, Gehalt
- Viele Probleme
- Oft interessant Zusammenhänge herauszufinden
  - Besonders warm an bestimmter Position
  - Mehr Gehalt bei Erfahrung oder bei vielen Treffern ?

### TABELLE
- Einfachste Form der Darstellung
- Hier: 15 Parameter Pro Messung
- Informationen lassen sich nur sehr schwer lesen
- Zusammenhänge kaum zu erkennen
- Meist liegen Daten in solcher Form vor

### KOMPRIMIERTE TABELLE
- Daten werden komprimiert
- Pro Parameter ein Balkendiagramm
- Mehr Daten können eingesehen werden
- BeispielDatensätze hier gezeigt (Wade Boggs & Don Mattingly)

### Streudiagramm Matrix
- Zeigt die Korrelation von x (hier 4) Parametern
- Somit Summe von k=1 bis n-1 (= (n(n-1))/2) Streudiagramme
- Wobei die Hälfte nur gespiegelt ist
- Auf der Diagonalen kann diverses stehen
  - Boxplots, Dichteschätzungen oder wie hier Gesamtverteilungen
- Bei vielen Parametern schnell unübersichtlich
- Interessante Datenstrukturen können nicht sichtbar werden
  - nur p(p-1)/2 Projektionen
  - z.B. "Grand Tour"
    - Streudiagramme im Dreidimensionalen
    - Parameter werden nach Betrachtung ausgetauscht (einzeln)
    - Alle Varianten durchprobieren um nichts zu übersehen

-> Weitere Möglichkeit

### Parallele Koordinaten
- Jede Achse stellt einen Parameter dar
- Ein Datensatz (hier blau) ist eine Linie, welche die Achsen schneidet
- Farbliche Gruppierung und Bündelung der Linien zur Vereinfachung
- Einfache Klusterfindung
- Skaliert gut mit hohe Dimensionen
- Mit Übung sind Strukturen gut zu erkennen
- Da höhere Dimensionen zweidimensional abgebildet werden tritt Informationsverlust auf
- Anordnung, Rotation und Skalierung der Achsen verändern das Bild
  - Ermöglichen unterschiedliche Blickwinkel
  - Schieriger zu Interpretieren

-> Ausreichend Darstellungsformen für multidimensionale Daten an die Hand gegeben.

## ZUSAMMENFASSUNG
