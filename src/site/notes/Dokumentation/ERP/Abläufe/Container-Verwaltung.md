---
{"dg-publish":true,"dg-path":"ERP/Abläufe/Container-Verwaltung.md","permalink":"/erp/ablaeufe/container-verwaltung/"}
---

# Container-Verwaltung

Mandant -- Kunde -- Lieferadresse 

1. Bestellung von Lieferadresse
	1. Preis(modell) Lieferadaresse 
2. Auftrag an Kunde 
3. Aufstellung und Abholung Lieferadresse
4. Rechnung an Kunde 
	1. Abrechnung gem. Preismodell Lieferadresse 

## Preismodell
![Pasted image 20231116153256.png](/img/user/Assets/Pasted%20image%2020231116153256.png)
Preismodelle werden in den eigens dafür vorgesehenen Modul erfasst. Hier besteht eine Beziehung aus der ID bzw. dem Namen des Preismodells und einem oder mehreren Artikeln. 

Wir einer dieser Artikel in einen Auftrag übernommen, wird in den Preismodellen nach einem passenden Eintrag gesucht und eingetragen. 

Da die Preismodelle zu den Lieferadressen eingetragen werden, beziehen sich diese nicht auf auf den Kunden, sondern auf den Kunden des Kunden. 
## An- und Abfahrt 
Es werden optional Fahrtkosten berechnet. Dies wird in der Adresse entschieden und entsprechend gesetzt. Die sich ergebenden Kosten sind in Zonen in der [[Dokumentation/ERP/Module/Administration#Tarifverwaltung\|Administration#Tarifverwaltung]] hinterlegt, welche ebenfalls in der Adresse ggffls. auszuwählen sind. 

> [!Hinweis]
> Über die Parameter `CONT_ABHOLUNG` und `CONT_ANLIEFERUNG` werden die Artikelnummern bestimmt, die eine Abrechnung beinhalten. Es wird aber ausschließlich beim Abholen/Anliefern und verwenden Webapp aufgeschlagen! 


