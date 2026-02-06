# Geodateninfrastruktur Winterthur: Normen, Standards und Applikationen mit Wartungsvertrag

Dieses Dokument gibt eine Zusammenstellung der in der **Geodateninfrastruktur Winterthur (GDIW)** verwendeten **Normen und Standards** sowie der **zentralen Applikationen mit laufendem Wartungsvertrag**. Es dient als Referenz für Betrieb, Beschaffung und Zusammenarbeit innerhalb der Stadtverwaltung Winterthur sowie mit externen Partnern.

## Abkürzungsverzeichnis

| **Abkürzung** | **Bedeutung**                                                                                              |
|---------------|----------------------------------------------------------------------------------------------------------|
| **AV**        | Amtliche Vermessung                                                                                     |
| **AVGBS**     | Schnittstelle zwischen Amtlicher Vermessung und Grundbuch                                               |
| **BfS**       | Bundesamt für Statistik                                                                                 |
| **CSW**       | Catalogue Services for the Web                                                                         |
| **DM01AVCH24**| Datenmodell der Amtlichen Vermessung des Kantons Zürich                                                |
| **DXF**       | Drawing Interchange Format                                                                              |
| **eCH**       | E-Government Standards Schweiz                                                                          |
| **FME**       | Feature Manipulation Engine                                                                          |
| **GeoJSON**   | Geospatial JavaScript Object Notation                                                                   |
| **GIS**       | Geoinformationssystem                                                                                   |
| **GML**       | Geography Markup Language                                                                               |
| **GWR**       | Gebäude- und Wohnungsregister                                                                           |
| **ISO**       | International Organization for Standardization                                                          |
| **JSON**      | JavaScript Object Notation                                                                              |
| **OGC**       | Open Geospatial Consortium                                                                              |
| **RFC**       | Request for Comments                                                                                    |
| **SIA**       | Schweizerischer Ingenieur- und Architektenverein                                                        |
| **sedex**     | Secure Data Exchange                                                                                    |
| **WFS**       | Web Feature Service                                                                                     |
| **WMS**       | Web Map Service  

## Normengerechte Bereitstellung von Applikationen

| **Norm**                     | **Erläuterungen**                                                                                                                                                         | **Einsatzbeispiel**                                                                 |
|-------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------|
| **Web Map Service (WMS)**    | Internationaler Standard (OGC 06-042) für Online-Kartendienste. Unterstützt von diversen GIS-Systemen.                                                                    | Bereitstellung der digitalen Karten des  Stadtplans als WMS-Dienste. Eine Übersicht der öffentlich bereitgestellten WMS-Dienste des Stadtplans kann unter folgendem Link abgerufen werden: https://stadt.winterthur.ch/themen/leben-in-winterthur/planen-und-bauen/wir-beraten-sie/geoinformation-und-vermessung/2d-stadtplan/2d-stadtplan-datenbeschreibung |
| **Web Feature Service (WFS)** | Standard (OGC 04-094) für Web-basierte Bereitstellung von Geodaten als Vektorgeometrien. Unterstützt von diversen GIS-Systemen.                                            | Von der GDIW aus wird ein öffentlich zugänglicher WFS-Dienst auf Wunsch der Bibliothek Zürich bereit gestellt: https://stadtplan.winterthur.ch/wfs/StadtkreiseWFS?SERVICE=WFS&VERSION=1.1&REQUEST=getCapabilities        |
| **CityGML**                  | Standard (OGC 12-019) für 3D-Stadtmodelle basierend auf GML (ISO 19136-1).                                                                                              | Das 3D-Stadtmodell kann über das folgende Online-Bestellformular extern explizit im CityGML-Format bestellt werden: https://stadt.winterthur.ch/themen/leben-in-winterthur/planen-und-bauen/geoinformation-und-vermessung/bestellungen/digitale-geoinformationen                                  |
| **GML Simple Feature Profile (GML-SF)** | Standard (OGC 06-103r4) zur Modellierung von Geodaten-Objekten mit Vektorgeometrie.                                                                                   | Verwendung beim oben genannten WFS-Dienst.                                                      |
| **Drawing Interchange Format (DXF)** | Standard für technische Zeichnungen aus dem CAD-Bereich, entwickelt von Autodesk.                                                                                     | Daten der AV werden bei der Stadtverwaltung häufig im DXF-Format bestellt und geliefert.                             |
| **GeoJSON**                  | Standard (RFC 7946) für den Austausch von Geodaten auf Basis von JSON.                                                                                                  | Einsatz in der Spielplatzkontrolle-Web-App.                                       |
| **Interlis**                 | Formale Sprache für die Modellierung und den Austausch räumlicher Daten.                                                                                                | Austausch von Geodaten der AV zwischen Stadt Winterthur und Kanton Zürich.                            |
| **DM01AVCH24**               | Datenmodell der AV des Kantons Zürich in Version 24.                                                                                                   | Erweiterung des Bundesdatenmodells durch Kanton Zürich.                                               |
| **SIA 405**                  | Datenmodell für den Austausch von Leitungsdaten in der Schweiz basierend auf Interlis.                                                                                   | Integration von Swisscom-Daten in die städtische Geodateninfrastruktur.            |
| **AVGBS**                    | Schnittstelle für den Datenaustausch zwischen AV und Grundbuch.                                                                                        | Datenaustausch zwischen Vermessungsabteilung Winterthur und Grundbuchamt Winterthur.                    |
| **Merkmalskatalog GWR**      | Objektklassen für den Austausch von Daten über Gebäude und Wohnungen (BfS).                                                                                              | Austausch von Geodaten zwischen Stadtverwaltung Winterthur und BfS.                                   |
| **eCH-0216**                 | Schnittstellenstandard für den Datenaustausch mit dem GWR.                                                                                                              | Austausch von Geodaten zwischen Stadtverwaltung Winterthur und BfS.                                                      |
| **Sedex**                    | Plattform des BfS für den sicheren Datenaustausch.                                                                                                                            | Sicherer Austausch von Geodaten zwischen Stadtverwaltung Winterthur und BfS.                                |
| **ISO 19115**                | Vorgaben zur Beschreibung geographischer Datensätze.                                                                                                                    | Geometadaten-Austausch zwischen Stadt Winterthur und BfS.                                             |
| **ISO 19139**                | XML-Schema-Definition für ISO 19115.                                                                                                                                     | Geometadaten-Austausch zwischen Stadt Winterthur und BfS.                                   |
| **OGC CSW**                  | Webservice zur Bereitstellung von Metadaten nach ISO 19139/19115.                                                                                                        | Indirekte Nutzung durch Bereitstellung von Winterthurer Geometadaten im Geometadaten-Katalog geocat.ch des BfS.                                    |

## Applikationen für die Geodateninfrastruktur Winterthur mit laufendem Wartungsvertrag

Die folgende Tabelle enthält eine möglichst vollständige Übersicht derjenigen **Applikationen** der Stadtverwaltung Winterthur, die von der **Fachstelle Geoinformation** betrieben werden und zu denen **regelmässige Zahlungen** z.B. für Wartung oder Lizenzen an externe Partner erfolgen. Diese öffentliche Publikation soll der **Transparenz über Lieferantenbeziehungen und der externen Abhängigkeiten** dienen.

| Applikation                                     | Einsatzzweck                               | Anbieter          | Hauptsitz              |
| ----------------------------------------------- | ------------------------------------------ | ----------------- | ---------------------- |
| Stadtplan Winterthur                            | Öffentliche Web-GIS-Applikation            | sourcepole AG     | 🇨🇭 Zürich, Schweiz      |
| Diverse AutoCAD Map Fachschalen                 | Leitungskataster, Strassenmanagement u.a.  | Geobox AG         | 🇨🇭 Winterthur, Schweiz  |
| Digitilt Inklinometer und Reader                | Inklinometermessungen                      | GeoSolutions International Ltd.  | 🇨🇭 Othmarsingen, Schweiz   |
| TBview                                          | Intranet-WebGIS-Client & Viewer            | GERST engineering | 🇩🇪 Rheine, Deutschland  |
| FME                                             | ETL- und Automations-Platform für Geodaten | Safe Software     | 🇨🇦 Surrey, Kanada       |
| Diverse Autodesk-Applikationen (AutoCAD Map 3D) | CAD-/GIS-Authoring & Basis für Fachschalen | Autodesk          | 🇺🇸 San Francisco, USA   |
| ArcGIS                                          | Desktop- und Online-GIS                    | Esri              | 🇺🇸 Redlands, USA        |
| rmGEO, Reality3D                                | Punktwolken-Verarbeitung, vermessungstechnische Auswertungen | rmData         | 🇦🇹 Pinkafeld, Österreich |
| Jira                                            | Ticket- und Kollaborations-Plattform       | Atlassian         | 🇦🇺 Sydney, Australien   |
| RealWorks, Business Center u.v.w.m.             | Auswertung und Verarbeitung von Punktwolken, Geländedaten, Totalstation etc.  | Trimble via allnav  | 🇺🇸 Westminster, USA   |
| Mavic 3E RTK  | Drohne mit RTK-Modul  | DJI via allnav | 🇨🇳 Shenzhen, China   |

Die hier gelisteten Produktnamen sind eingetragene Marken der jeweiligen Unternehmen. Die Stadt Winterthur erhebt keinen Anspruch auf diese Marken.
