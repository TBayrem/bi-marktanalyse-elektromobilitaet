# Elektromobilität im Datencheck: Ein Power-BI-Dashboard für einen Energiekonzern

*Von Bayrem Trabelsi, gemeinsam mit Sarah Hauschildt und Tsopfack Sofo Romi. Projektbericht im Modul Business Intelligence (M.Sc. Wirtschaftsinformatik, Hochschule Worms, WiSe 2024/25, Betreuung: Prof. Dr. Paul Langer). PhotoWin Energy ist ein fiktiver Fall.*

---

## Die Frage

Ein Energiekonzern mit Know-how in Wind- und Solarenergie überlegt, in die Elektromobilität einzusteigen. Die Hürden sind bekannt: zu wenig Ladeinfrastruktur, hohe Strompreise beim Schnellladen und Reichweite (zur Marktentwicklung siehe [1]). Wir sollten mit Daten eine Entscheidungsgrundlage liefern.

## Vom Rohdatensatz zum Dashboard

**Quellen:** das Ladesäulenregister der Bundesnetzagentur [2] (offene Daten unter Creative-Commons-Lizenz) sowie mehrere Marktstatistiken zu Bestand, Prognose, Batteriepreisen und Herstellern, Strompreisen und Kaufbarrieren.

**ETL in Power Query** [3]:
1. Extract: Daten aus Excel und CSV laden, Struktur in der Vorschau prüfen.
2. Transform: Datentypen korrigieren, Leerwerte und Duplikate entfernen, Spalten ableiten (zum Beispiel das Jahr aus einem Datum), Währungen vereinheitlichen, Testdaten filtern.
3. Load: bereinigte Daten ins Datenmodell laden und prüfen.

**Das Dashboard** besteht aus zehn Grafiken, unter anderem E-Autos pro Bundesland, Bestandsentwicklung mit Prognose bis 2035, Schnell- und Normalladepunkte im Zeitverlauf, Strompreise AC und DC nach Betreiber, Batterieproduktion nach Hersteller, Lithium-Ionen-Preise, Produktionskapazität nach Region, Gründe gegen den E-Auto-Kauf und Belegung öffentlicher Ladepunkte.

## Was die Daten zeigen

- Die Zahl der Ladepunkte hält mit dem Wachstum der E-Autos nicht Schritt, vor allem auf dem Land.
- Schnellladen liegt preislich bei 0,50 bis 0,75 € pro kWh und kann Nutzer abschrecken.
- Lithium-Ionen-Akkus dominieren, Natrium-Ionen-Akkus gewinnen an Bedeutung.
- Die Batterieproduktion wird stark von China dominiert.
- Umfragen zeigen höhere Reichweitenwünsche, als viele Modelle bieten.

## Vier Handlungsoptionen

| Option | Idee |
|---|---|
| 1 Batterien | Forschung an Lithium-, Natrium- und Silizium-Ionen-Akkus mit mehr Reichweite |
| 2 Solarfolie | Folie am Fahrzeug nutzt die Solar-Kompetenz und lädt die Batterie nach |
| 3 Ladesäulen | Schnelllader an Autobahnen und Kundenparkplätzen, Normallader für Firmen, Kooperationen mit Supermärkten, ausgehandelte Stromtarife |
| 4 HomePorts und Tarife | Wallboxen beim Kunden, Vergünstigungen und Zusatztarife für E-Auto-Fahrer |

## Was die Arbeit nicht leistet

- Die vier Optionen sind **nicht bewertet oder gewichtet**. Ein Scoring (wie in meiner Digital-Twin-Fallstudie) wäre der logische nächste Schritt.
- Es gibt **keinen Business Case** mit Investitionen und Erträgen.
- Der Reichweitengewinn der Solarfolie ist **nicht quantifiziert**.

## Was ich mitnehme

- **Ein Dashboard braucht eine Entscheidungsfrage.** Zehn Grafiken sind nur nützlich, wenn jede eine konkrete Frage beantwortet.
- **ETL ist der größte Teil der Arbeit.** Saubere Daten entscheiden über die Qualität jeder Analyse.
- **Von der Analyse zur Empfehlung braucht es Zahlen:** Kosten, Nutzen und Risiken pro Option.

## Quellen

1. IEA (2024): Global EV Outlook 2024. Paris. https://www.iea.org/reports/global-ev-outlook-2024
2. Bundesnetzagentur: Elektromobilität, Öffentliche Ladeinfrastruktur (Ladesäulenregister). https://www.bundesnetzagentur.de/ladeinfrastruktur
3. Microsoft: Power-Query-Dokumentation. https://learn.microsoft.com/de-de/power-query/

*Hinweis: Preise, Herstellerangaben und Aussagen zu Produkten geben den Stand der jeweiligen Studienarbeit wieder. Alle Links wurden zuletzt im November 2026 gesucht oder abgerufen; Quellen mit dem Vermerk "wie in der Studienarbeit zitiert" sind dort im Literaturverzeichnis nachzuschlagen.*

---

*Ich suche zum 01.03.2027 den Einstieg als Junior IT Consultant oder IT Business Analyst. [LinkedIn](https://linkedin.com/in/bayremtrabelsi)*