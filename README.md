# nominatim
Nominatim ist eine Open-Source-Geokodierungssoftware, die auf OpenStreetMap (OSM)-Daten basiert. Sie ermöglicht:

- Geokodierung – Umwandlung von Adressen oder Ortsnamen in Koordinaten.
- Reverse-Geokodierung – Ermittlung einer Adresse oder eines Ortes aus Koordinaten.
- Suche nach Orten – Finden von Städten, Straßen oder POIs (Points of Interest).

### Einsatz im Projekt

Beim MLA wird Nominatim dazu genutzt um Geokoordinaten mit Adressinformationen anzureichern. Das bedeutet, dass Sensoren, Messwerte oder Points of Interest (POIs), die nur als Breiten- und Längengrad vorliegen, durch eine Reverse-Geokodierung mit menschenlesbaren Adressen ergänzt werden.
Anwendungsfälle in MLA:

- Verkehrssensoren: Ergänzen von Positionsdaten mit Straßen- oder Ortsnamen.
- Umweltmesswerte: Verknüpfen von Luftqualitäts- oder Wetterdaten mit Stadtteilen oder Postleitzahlen.

Das verbessert die Lesbarkeit und ermöglicht bessere Analysen, etwa zur Stadtplanung.



## Voraussetzungen
* Kubernetes 1.30+

## TL;DR

Die Variablen im Manifest müssen zuvor entsprechend der eigenen Umgebung angepasst werden.

```bash
$ kubectl apply -f manifest/* -n nominatim --create-namespace
```

## Variablen
Die Nachfolgenden Variablen werden im Manifest verwendet.

| Name                    | Description                                     | Value  |
|:------------------------|:------------------------------------------------|:-------|
| CI_PROJECT_NAME         | Projektname                                     | []     |
| PBF_URL                 |                                                 | []     |
| REPLICATION_URL         |                                                 | []     |
| MEM_REQUEST             |                                                 | []     |
| CPU_REQUEST             |                                                 | []     |
| MEM_LIMIT               |                                                 | []     |
| CPU_LIMIT               |                                                 | []     |

## Links
https://wiki.openstreetmap.org/wiki/Nominatim
https://download.geofabrik.de

## License
Copyright © 2024 ADDIX GmbH.