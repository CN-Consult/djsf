# DJSF 
This repository contains all information about the **D**iLoc**J**son**S**chedule**F**ormat.

[DJSF-Schema interactive online viewer](https://diloc.de/wp-content/uploads/djsf/#https://raw.githubusercontent.com/CN-Consult/djsf/master/djsf.json)

## Changelog
- **v0.1.1**
    - Initiale Version.
- **v1.0.0**
    - Implementierung RouteStationIdentifier
        - stations umbenannt zu RouteStations
        - stations.station umbenannt zu RouteStations.RouteStationIdentifier
        - RouteStationIdentifier ist nun ein Objekt
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
    - Added support for pre announcements.
    - Enhanced description for 'on'-paramenter of a command. 
    - Added optional 'timeoffset' parameter. 
- **v2.2.0** 
    - Added piNumber to trains
- **v2.3.0** 
    - Added support for multitraction trains.
- **v2.3.1** 
    - Specified timeTableArrivalTime and timeTableDepartureTime more precise.
- **v2.3.2** 
    - Fixed enum value for period schedule
                