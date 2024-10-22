---
{"dg-publish":true,"dg-path":"/ERP/Stammdaten/Kunden","dg-permalink":"/ERP/Stammdaten/Kunden","permalink":"/ERP/Stammdaten/Kunden/"}
---

# Stammdaten Kunden

Die Stammdaten enthalten alle erdenklichen Angaben zu jedem Kunden. Neben reinen Informationen sind hier auch wesentliche Merkmale wie Kundengruppen, Zahlungs- und Lieferbedingungen, Währungen etc. enthalten, welche einen Geschäftsprozess erst möglich machen. So gesehen gibt es Pflichtfelder, welche aber nicht als solche gekennzeichnet sind. 
Da es selbsterklärende Felder wie Namen und Adresse gibt, wird hier nun nicht jedes beschrieben, sondern es wird auf Besonderheiten und nennenswerte Hinweise fokussiert.  

![Stammdaten_Kunden.png](/img/user/Assets/Stammdaten_Kunden.png)
- ( 1 ) Neben dem Hinzufügen per Drag&Drop ist es über die TWAIN-Scanner-Schnittstelle möglich, dem Kunden Dokumente anzuhängen. 
- ( 2 ) Für Verkaufsbelege lassen sich automatische in die jeweiligen Belegtyen einzutragende Kopf- und Fußtexte definieren. 
- ( 3 ) Hier werden die Änderungen des Kundendatensatzes protokolliert 
- ( 4 ) Es lässt sich eine explizite Adresse nur für den Rechnungsversand vergeben
- ( 5 ) Geprüft ist eine Infofeld, inaktiv verhindert das Vorkommen in der Suche und gesperrt verbietet das Anlegen von Belegen 
- ( 6 ) Soll ein Entsorgungsnachweis erstellt werden? Wenn ja, dann
  - ![Pasted image 20231116123829.png](/img/user/Assets/Pasted%20image%2020231116123829.png)
- Zudem ist die Angabe möglich. ob Container gemietet werdern können und ab welcher Anzahl Tage Miete berechnet wird 
- ( 7 ) Für die Conainerverwaltung kann festgelegt werden ob und an wen eine Lieferscheinkopie gesendet wird. 
- ( 8 ) Hier wird die Kommissionierung einer Bestellung aktiviert. Per Scanner werden KLTs den Auftragspositionen zugwiesen 
- ( 9 ) Handelt es sich bei diesem Kontakt um eine Spedition? 
- ( 10 ) In welchem Bereich ist der Kontrakt tätig? 
- ( 11 )  In den Parametern definierte Multiselektion (`AP_CHECK#`)

> [!Hinweis]
> Teilweise sind Felder nicht editierbar, dann ist hier ein externe Anbindung konfiguriert. Diese kann mit dem folgenden Parameter in der [[Dokumentation/ERP/📚 Module/Administration#Parameterverwaltung\|Administration#Parameterverwaltung]] geändert werden, 
> 
> `SAGE_KDIMP = false`
## Adressen 
Hier finden sich weitere, über die Hauptadresse hinaus gehende Adressen. Sie sind für die Verwendung in Lieferscheinen oder Rechnungen vorgesehen. Bei identischen Adressen für Lieferung und Rechnungen sind diese doppelt anzulegen.
![Pasted image 20231116130128.png](/img/user/Assets/Pasted%20image%2020231116130128.png)
- ( 1 ) Das [[Dokumentation/ERP/Abläufe/Container-Verwaltung#Preismodell\|Container-Verwaltung#Preismodell]] bestimmt den Preis für den Kunden des Kunden, also den Kunden gem. Lieferadresse 
- ( 2 ) Ein optionale Vertreter ist eine Person, die an der Adresse eine Bedeutung hat. Dies kann ein Verantwortlicher sein, aber auch lediglich jemand, der einen Zugang verschafft 
- ( 3 ) An und Abfahrt können berechnet werden, dies wird je Adresse entschieden
- ( 4 ) Fotos können bspw. die Blumen sein, die im Rahmen einer Dienstleistung gepflegt werden. 
- ( 5 ) Dokumente können hier wie auch im Vorgang per Drag&Drop hinzugefügt werden 
## Offene Aufträge 
![Pasted image 20231116162229.png](/img/user/Assets/Pasted%20image%2020231116162229.png)
Ab  dieser Ansicht kann direkt in die Aufträge gesprungen werden. 
## Historie
![Pasted image 20231116162651.png](/img/user/Assets/Pasted%20image%2020231116162651.png)
Dies bietet eine komplette Übersicht aller den Kunden betreffenden Vorgänge, gefiltert auf ein Jahr. Das darzustellende Jahr wird über ein Ausklappmenü gewählt und ist zunächst immer das aktuelle. Auch hier ist natürlich ein Direktsprung in den Vorgang möglich. 
## Artikel 
![Pasted image 20231116163335.png](/img/user/Assets/Pasted%20image%2020231116163335.png)
Auf der Seite Artikel finden sich die kundenbezogenen Artikel mit Preis, Artikel- und Zeichnungsnummer. Ebenfalls können Preiseinheit, Mengenstaffel eingesehen werden. 
Erfasst werden diese Konditionen in [[Dokumentation/ERP/📚 Module/Stammdaten/Artikel\|Artikel]].
### Zuschl. ber

### Gesamtbestand
Der aus allen Lägern zusammengefasste Bestand. 
### Archiviert 
Artikel können im Artikelstamm ins Archiv verschoben werden. 
![Pasted image 20231116170041.png](/img/user/Assets/Pasted%20image%2020231116170041.png)
Sie sind dann nicht mehr sicht- und verwendbar, jedoch in dieser Ansicht entsprechend markiert. 

## E-Mails
Es werden die über dieses Programm gesendete und empfangene E-Mais aufgeführt. 
## Kennzahlen 
Ein schneller Überblick über die relevantesten Zahlen des Kunden. Verglichen mit dem Vorjahr und gefiltert auf ein Werk. Das Werk ist auswählbar. 
## Dokumente 
Alle dem Kunden zugeordnete Dokumente. Mit einer Vorschau des gewählten Dokuments auf der rechten Seite. 
## Werkezuordnung 
Die Spalte **Werke-Nr** identifiziert das eigene Werk. **aktiv** ist eine Selektionskriterium bspw. für Formularauswahl bei Kampagnen.  

Je Werk kann eine **Eigene KundenNr** eingetragen werden, dies ist die Nummer, der der Kunde für dieses Werk in seinen Systemen führt. 

Zudem kann je Werk eine E-Mail-Adresse für den Rechnungsversand bestimmt werden.
## Lademittel 
![Pasted image 20231116171958.png](/img/user/Assets/Pasted%20image%2020231116171958.png)
Im oberen Fenster ist der Saldo des Lademittels zu erkennen. Mit positive Zahl ist "haben" eine negative "soll".
Im unteren Fenster wird gebucht. Zugang ist hier ein Erhalt vom Kunden, also eine Buchung ins Soll, Abgang bedeutet eine Rückgabe an den Kunden. 

> [!Hinweis]
> Wenn hier die Zahl bei bspw. KLTs größer Null wird, wurde mehr zurück gegeben, als entgegen genommen wurde. Hier besteht dann der Verdacht von Fehlbuchungen. 
