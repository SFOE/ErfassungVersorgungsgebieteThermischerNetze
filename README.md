# Erfassung Geodaten Versorgungsgebiete Thermischer Netze
Der Verband Thermische Netze Schweiz und das Bundesamt für Energie erstellen eine Übersicht aller Gebiete mit bestehender und geplanter Fernwärmeversorgung. Die Geodaten werden von den Anlagebetreibenden gemäss minimalem Geodatenmodell erfasst. Hier finden Sie nützliche Informationen welche bei der Erfassung der Geodaten helfen können.

* [Minimales Geodatenmodell]()
* [INTERLIS - Allgemeine Informationen]()

Bei Fragen oder Unklarheiten erstellen Sie einen [Issue]([https://github.com/SFOE/GeodatenschnittstelleDokumentation/issues](https://github.com/SFOE/ErfassungVersorgungsgebieteThermischerNetze/issues)) oder schreiben Sie eine [E-Mail](mailto:geoinformation@bfe.admin.ch)



## Minimales Geodatenmodell
Das minimale Geodatenmodell (MGDM) und die Dokumentation finden Sie hier:
* [Minimales Geodatenmodell](https://github.com/SFOE/ErfassungVersorgungsgebieteThermischerNetze/blob/main/files/SupplyTerritoriesOfThermalNetworks_V1.ili)
* [Dokumentation minimales Geodatenmodell](https://github.com/SFOE/ErfassungVersorgungsgebieteThermischerNetze/blob/main/files/Versorgungsgebiete%20thermischer%20Netze%20DE%20V1.pdf)
* *Die Publikation des MGDM im Model Repository folgt.*
* *Die Publikation der externen Kataloge folgt.*

## INTERLIS - Allgemeine Informationen
Die Geodaten müssen in INTERLIS erstellt werden. Hier finden Sie allgemeine Informationen zu INTERLIS:
* [Referenzhandbuch](https://www.interlis.ch/dokumentation/interlis-2)

## INTERLIS - Geodaten erfassen
Folgende Werkzeuge eignen sich für die Erstellung von INTERLIS-Geodaten:

### QGIS Model Baker
* Das Model Baker Plugin kann direkt in QGIS über *Erweiterungen verwalten und installieren* installiert werden.
* [Dokumentation](https://opengisch.github.io/QgisModelBaker/de/)

### FME mit dem Plugin ili2fme
* Mit dem Plugin *ili2fme* können INTERLIS-Daten in FME gelesen und geschrieben werden.
* [Download](https://www.interlis.ch/downloads/ili2fme)
* [Dokumentation](https://www.geo.admin.ch/de/geodatenmodelle/)
* *FME-Vorlage folgt*

### ili2db - Ladeprogramm für Datenbanken (PostgrSQL/PostGIS, GeoPackage oder ESRI FileGDB)
* Mit ili2db kann ein modellkonformes Datenbankschema erstellt werden. Aus diesem Datenbankschema können anschliessend valide INTERLIS-Daten exportiert werden.
* [Download](https://www.interlis.ch/downloads/ili2db)
* *Datenbankschema folgt*

## INTERLIS - Geodaten validieren
INTERLIS-Geodaten können mit folgenden Werkzeugen validiert werden:
* [ilicop.ch](https://ilicop.ch/)
* [ilivalidator](https://www.interlis.ch/downloads/ilivalidator)
* [iGCheck](https://www.interlis.ch/downloads/igcheck)

## Geodaten publizieren
Valide Geodaten können Sie dem Bundesamt für Energie über die [Geodatenschnittstelle](https://github.com/SFOE/GeodatenschnittstelleDokumentation) übermitteln.
