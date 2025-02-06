# nominatim
 Open-source geocoding with OpenStreetMap data

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