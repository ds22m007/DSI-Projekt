# DSI - Projekt
von Dominik Meisel, Andreas Stern und Samuel Pernthaler.

# Architektur
[![Architektur](https://raw.githubusercontent.com/ds22m007/DSI-Projekt/main/dsi_architecture.drawio.png))

Datenquellen sind die Twitter-Api & Aktienkurse von Tesla (Yahoo Finance)

Diese werden in Kafka geschrieben und mit Apache Spark (Streaming) aggregiert in eine Influx DB geschrieben.
Zur Visualisierung wird Grafana verwendet!

## Dashboard für Aktienkurse
Es soll ein Dashboard geschaffen werden, das TSLA Aktienkurse in Relation zu Daten von Twitter Inc. zeigt. Dazu werden Kursdaten der TSLA-Aktie aus vergangenen Jahren verwendet.

Im Vergleich dazu sollen Twitter-Daten der public-API herangezogen werden, um eine Beziehung zwischen den beiden Datensets herzustellen. Die Twitter-API bietet diverse Daten an, die für die Erklärung von Aktienkursen dienen können. Unter anderem kann die Anzahl der Tweets an einem Tag zu einem Hashtag zeigen, ob es gerade eine breite öffentliche Diskussion zum Unternehmen gibt. 

