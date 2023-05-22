# DJSF 
Dieses Repository beinhaltet alle Informationen über das **D**iLoc**J**son**S**chedule**F**ormat.

This repository contains all information about the **D**iLoc**J**son**S**chedule**F**ormat.

[DJSF-Schema interactive online viewer](https://diloc.de/wp-content/uploads/djsf/#https://raw.githubusercontent.com/CN-Consult/djsf/master/djsf.json)

## Changelog
### Deutsch
- **v0.1.1**
    - Initiale Version.
- **v1.0.0**
    - Implementierung RouteStationIdentifier
        - stations umbenannt zu RouteStations
        - stations.station umbenannt zu RouteStations.RouteStationIdentifier
        - RouteStationIdentifier ist nun ein Objekt mit den folgenden Werten:
            - string: idCode
            - number: sequenceNumber
- **v1.0.1**
    - Id's gefixt und Kompatibilität geprüft. 
      - Diese Version ist nun kompatible zu lbovet/docson
      - Verbesserte Dokumentation vom Tag "meta"
      - Tag "djsfSchemaVersion" hinzugefügt und dokumentiert.
- **v1.1.0**
    - Files-Array hinzugefügt, welches alle Dateinen die im Fahrplan genutzt werden enthält.
- **v2.0.0**
    - Typ "integer" für Parameter "on" hinzugefügt.
    - RouteStationIdentifier ist nun ein eigener Objekt-Typ.
    - Die Station unterhalb von script tracks ist nun ein RouteStationIdentifier.
- **v2.1.0** 
    - Unterstützung für Begrüßungsansagen hinzugefügt.
    - Erweiterung der Beschreibung des 'on'-Parameters für einen Command.
    - Unterstützung eines 'timeoffset'-Parameters für einen Command.
- **v2.2.0** 
    - piNumber(passenger-information-number) hinzugefügt.
- **v2.3.0**
    - Unterstützung für Fahrten in Multitraktion hinzugefügt.
- **v2.3.1** 
    - Spezifikation für timeTableArrivalTime timeTableDepartureTime angepasst. 
- **v2.3.2** 
    - Enum-Wert für Jahresfahrplan behoben. 
- **v2.4.0** 
    - Unterstützung des Zug-Verbindungstyps 'Durchbinden' hinzugefügt.                  
- **v2.4.1** 
    - 'train' aus nextTrainNumber und nextTrainLinkType entfernt, weil es redundant ist.
    - nextPiNumber hinzugefügt  
- **v2.4.2**
    - createdAt für Erzeugungszeitpunkt des Fahrplans hinzugefügt.
- **v2.4.3**
    - 'fileDownloadUrl' in meta daten hinzugefügt
         
### English
- **v0.1.1**
    - Initial version.
- **v1.0.0**
    - Implemented RouteStationIdentifier.
        - renamed stations to RouteStations.
        - renamed stations.station to RouteStations.RouteStationIdentifier.
        - RouteStationIdentifier is now an object with the following members:
            - string: idCode
            - number: sequenceNumber
- **v1.0.1**
    - Fixed ids and checked compatibility.
        - this version is now compatible with lbovet/docson.
        - improved documentation of the meta-tag.
        - added djsfSchemaVersion.
- **v1.1.0**
    - Added files-array which contains all referenced files in the schedule.
- **v2.0.0**
    - Added type 'integer' for 'on'-parameter.
    - RouteStationIdentifier is now an own object.
    - The station of script-tracks is now a RouteStationIdentifier.
- **v2.1.0** 
    - Added support for pre announcements.
    - Enhanced description for 'on'-paramenter of a command. 
    - Added optional 'timeoffset' parameter. 
- **v2.2.0** 
    - Added piNumber to trains.
- **v2.3.0**
    - Added support for multitraction trains.
- **v2.3.1**  
    - Specified timeTableArrivalTime and timeTableDepartureTime more precise.
- **v2.3.2**  
    - Fixed enum value for period schedule
- **v2.4.0** 
    - Added support for train link type 'continuation'.                 
- **v2.4.1** 
    - removed 'train' from nextTrainNumber and nextTrainLinkType because it is redundant
    - added nextPiNumber 
- **v2.4.2**
    - Added 'createdAt' which represents the generation timestamp of the schedule.
- **v2.4.3**
    - Added 'fileDownloadUrl' to meta data
