# Erfassung Geodaten Versorgungsgebiete Thermischer Netze
Der Verband Thermische Netze Schweiz und das Bundesamt für Energie erstellen eine Übersicht aller Gebiete mit bestehender und geplanter Fernwärmeversorgung. Die Geodaten werden von den Anlagebetreibenden gemäss minimalem Geodatenmodell erfasst. Hier finden Sie nützliche Informationen welche bei der Erfassung der Geodaten helfen können.

* [Minimales Geodatenmodell](https://github.com/SFOE/ErfassungVersorgungsgebieteThermischerNetze/tree/main#minimales-geodatenmodell)
* [INTERLIS - Allgemeine Informationen](https://github.com/SFOE/ErfassungVersorgungsgebieteThermischerNetze/tree/main#interlis---allgemeine-informationen)
* [INTERLIS - Geodaten erfassen](https://github.com/SFOE/ErfassungVersorgungsgebieteThermischerNetze/tree/main#interlis---geodaten-erfassen)
* [INTERLIS - Geodaten validieren](https://github.com/SFOE/ErfassungVersorgungsgebieteThermischerNetze/tree/main#interlis---geodaten-validieren)
* [Geodaten publizieren](https://github.com/SFOE/ErfassungVersorgungsgebieteThermischerNetze/tree/main#geodaten-publizieren)

Bei Fragen oder Unklarheiten erstellen Sie einen [Issue](https://github.com/SFOE/ErfassungVersorgungsgebieteThermischerNetze/issues) oder schreiben Sie eine [E-Mail](mailto:geoinformation@bfe.admin.ch)



## Minimales Geodatenmodell
Das minimale Geodatenmodell (MGDM) und die Dokumentation finden Sie hier:
* [Minimales Geodatenmodell](https://github.com/SFOE/ErfassungVersorgungsgebieteThermischerNetze/blob/main/files/SupplyTerritoriesOfThermalNetworks_V1.ili)
* [Dokumentation minimales Geodatenmodell](https://www.bfe.admin.ch/bfe/de/home/versorgung/statistik-und-geodaten/geoinformation/geodaten/thermische-netze/versorgungsgebiete-thermischer-netze.html)
* Kataloge
  * [SupplyTerritoriesOfThermalNetworks_EnergySource_Catalogue_V1.xml](https://github.com/SFOE/ErfassungVersorgungsgebieteThermischerNetze/blob/main/files/SupplyTerritoriesOfThermalNetworks_EnergySource_Catalogue_V1.xml)
  * [SupplyTerritoriesOfThermalNetworks_ObligationToConnect_Catalogue_V1.xml](https://github.com/SFOE/ErfassungVersorgungsgebieteThermischerNetze/blob/main/files/SupplyTerritoriesOfThermalNetworks_ObligationToConnect_Catalogue_V1.xml)
  * [SupplyTerritoriesOfThermalNetworks_SourceofHeat_Catalogue_V1.xml](https://github.com/SFOE/ErfassungVersorgungsgebieteThermischerNetze/blob/main/files/SupplyTerritoriesOfThermalNetworks_SourceofHeat_Catalogue_V1.xml)
  * [SupplyTerritoriesOfThermalNetworks_Status_Catalogue_V1.xml](https://github.com/SFOE/ErfassungVersorgungsgebieteThermischerNetze/blob/main/files/SupplyTerritoriesOfThermalNetworks_Status_Catalogue_V1.xml)
* [Testdaten in INTERLIS](https://uvek-gis.admin.ch/BFE/berichte/VersorgungsgebieteThermischerNetze/Testdaten_Interlis.zip)
* *Die Publikation des MGDM und der Kataloge im Model Repository folgt.*

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
* [FME-Template](https://uvek-gis.admin.ch/BFE/berichte/VersorgungsgebieteThermischerNetze/FME_Template_DE.zip)

### ili2db - Ladeprogramm für Datenbanken (PostgrSQL/PostGIS, GeoPackage oder ESRI FileGDB)
* Mit ili2db kann ein modellkonformes Datenbankschema erstellt werden. Aus diesem Datenbankschema können anschliessend valide INTERLIS-Daten exportiert werden.
* [Download](https://www.interlis.ch/downloads/ili2db)
* [Dokumentation](https://github.com/claeis/ili2db/blob/master/docs/ili2db.rst)

## INTERLIS - Geodaten validieren
INTERLIS-Geodaten können mit folgenden Werkzeugen validiert werden:
* [ilicop.ch](https://ilicop.ch/) (erst möglich sobald MGDM im Model Repository publiziert ist)
* [ilivalidator](https://www.interlis.ch/downloads/ilivalidator)
* [iGCheck](https://www.interlis.ch/downloads/igcheck)

## Geodaten publizieren
Valide Geodaten können Sie dem Bundesamt für Energie über die [Geodatenschnittstelle](https://github.com/SFOE/GeodatenschnittstelleDokumentation) übermitteln.
