# TimeBookerReleases
Contains the Releases for the private TimeBooker Repository https://github.com/Fleege/TimeBooker


## Anforderungen
Zum Start der Exe ist die .NET 6 Runtime erforderlich, die Exe weist auf eine fehlende Runtime beim Start hin und bietet die Installation automatisch an.

## Installation
Es muss einfach die Zip-Datei irgendwo entpackt werden, danach kann die TimeBooker.exe gestartet werden.

Die Datei `.\bookingTargets.json` definiert die zur Verfügung stehenden Buchungsziele, sie beinhaltet ein Array im JSON-Format mit den folgenden Eigenschaften je Element:
 - activityType: String der Leistungsart
 - internalOrder: String des Innenauftrags
 - description: Eine Beschreibung, dieses Feld darf leer sein

Zudem muss ein Ordner `.\timeTableEntries` existieren, in diesem werden json-dateien mit den gebuchten Zeiten vom Programm abgelegt

Beide Pfade können in der Konfigurationsdatei `TimeBooker.dll.config` angepasst werden