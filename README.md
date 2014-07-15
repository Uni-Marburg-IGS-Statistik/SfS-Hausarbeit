# Dichotomisierung quantitativer Variablen

Dichotomisierung, inkl. sog. Median-Splits, wandeln eine quantitative Variable in eine zweistufige Variable. Sie werden u.a. stark kritisiert, weil sie die Beziehung zwischen einzelnen Datenpunkte verzerren. Zum Beispiel werden bei Median Splits die zwei Werte, die unmittelbar auf beiden Seiten des Medians liegen, so ähnlich behandelt wie die zwei Extrema, obwohl sie eigentlich viel näher aneinander sind als an den Extrema. Historische Gründe dafür sind u.a. die Notwendingkeit kategorischer Variablen bei Verfahren wie ANOVA. Diese Praxis wird immer stärker in der [Literatur](http://dx.doi.org/10.1037/1082-989X.7.1.19) kritisiert, v.a. mit der praktischen Handhabung von Methoden wie gemischte Modelle, die sowohl mit Messwiederholung als auch Variablen aller Skaltenarten umgehen können. Hier werden Sie die Auswirkung der Dichotomisierung untersuchen, indem Sie folgende Verfahren anhand eines Datensatzes und deren Ergebnisse vergleichen:

1. ANOVA mit 
    a. mediangesplitter Variable
    b. meangesplitter Variable
2. gemischte Modelle mit 
    a. mediangesplitter Variable
    b. meangesplitter Variable
3. gemischte Modelle mit ursprünglischer quantitativer Variable
4. (optional) ANCOVA mit ursprünglischer quantitativer Variable

Sie haben freie Wahl des Datensatzes, aber das Design des Ausgangsexperiments muss mittels Messwiederholung ausgeführt worden sein. Weiterhin müssen Sie zumindest einen weiteren Faktor als die dichotomisierte Variable in Analyse aufnehmen. EEG-Experimente mit einer Frequenz-Manipulation und einer weiteren Manipulation, wie z.B. manche N400 Paradigma, wären geeignet; bei EEG-Experimente dürfte man sich auf eine Elektrode konzentrieren, damit die Topographie (ROI) die Analyse nicht erschwert. Bei Bedarf wird ein Datensatz, z.B. `priming.tab` aus der Kurs-Repository, zur Verfügung gestellt. 

Bei den einzelnen Verfahren sollten Sie auch die übliche Praxis und Standardsbeachten, z.B. Auflösung von Interaktionen in ANOVA, maximale RE-Struktur bei gemischten Modellen, usw.

Fragen, die durch die Untersuchung, behandelt werden sollten, sind:

1. Wie unterschieden sich die Ergebnisse aus ANOVA und den gemischten Modelle?
2. Wie unterschieden sich die zwei Dichotomisierungsarten?
3. Welche Auswirkung hat die Dichotomisierung bei neuartigen Verfahren (Vergleich der gemischten Modelle)? 
4. (optional) Welche Auswirkung hat die Dichotomisierung bei herkömmlichen Verfahren (Vergleich von ANOVA und ANCOVA)?

## Formalia
### Termine 
* Freischalttermin: Dienstag, 15.07.2014 um 10 Uhr (zum Beginn der Klausur)
  - Daten über GitHub herunterladen
  - Beim Erscheinen zum Klausurtermin Ausdruck des Aufgabeblatts auch verfügbar, sonst in der Repository 
* Abgabetermin: 31.08.2014

### Technische Aspekte
* Abgabge über Private-Repository unter der Uni-Marburg-IGS-Statistik-Organisation (wird von mir eingerichtet)
* Arbeit als RMarkdown gespeichert
* Metadaten angeben (vgl. [Dokumentation zu pandoc](http://johnmacfarlane.net/pandoc/README.html#title-block))  
    * Titel: Power-Verlust bei Median Splits: ein Vergleich zwischen ANOVA und gemischten Modellen
    * Author(in): `Anrede Nachname, Vorname <benutzername@students.uni-marburg.de>`
    * Darum `% 2014-MM-TT`
* einfache Lizenz im letzten Kapitel, z.B.: 
```
# Lizenz
Diese Datei darf weiter als anonymes Beispiel genutzt werden.
```
oder
```
# Lizenz
Diese Datei darf nur zu Prüfungszwecken dienen.
```



