# Datensatz OceanRace #
Codebuch Stand 2025-01
erstellt von Team Ocean Race (Ansprechpartnerin Viktoria Reiser vr047@hdm-stuttgart.de)

## Inhalt
- Edgelist_OceanRace.csv (Edgelist)
- Nodelist_OceanRace.csv (Nodelist)
- OceanRace.rmd (Markdown-Dokument)
- Codebuch.md (Codierung der Datensätze)

## Ursprung und Datenerhebung
Wir haben einen Datensatz für den Pretest eines Netzwerks von "the Ocean Race" aus den Episoden 2014/15 und 2017/18 erhoben. Die Daten haben wir auf der offiziellen Webseite von Ocean Race, den entsprechenden Wikipedia-Artikeln und einzelnen Webseiten zu den Teams gefunden. 

Das Netzwerk ist ein *gerichtetes three-mode Netzwerk*, das sich in zwei Arten von Netzwerke gliedern lässt. 

1) Ein Zusammenarbeitsnetzwerk *team*, das die Verbindung aller Segler aus den Jahren 14/15 und 17/18 zu ihren Teams darstellt.

2) Ein Nationalitätennetzwerk *nationality*, das die Verbindung aller Segler zu ihrer Nationalität darstellt.

**Umgang mit fehlgenden Werten:**
Fehlende Werte werden nicht erfasst.

# EDGE-Attribute

**from**
initiierender Knoten, in diesem Fall: Segler

**to**
erhaltender Knoten, in diesem Fall: Team, in dem der Segler angetreten ist oder Nationalität des Seglers


# NODE-Attribute  
  
**id**    
Alphanumerisch: Initialen des Seglers (bei Dopplung wurde bei einem der Segler der zweite Buchstabe des Nachnamens ergänzt), als string/characters codiert 

**sailor**
Alphanumerisch: Voller Name des Seglers, als string/characters codiert


**position**    
Position auf dem Segel, als string/characters codiert 

  
**nationality**  
ISO-Code der Nationalitäten, als string/characters codiert


##
