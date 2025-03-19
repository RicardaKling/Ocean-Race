# Datensatz OceanRace #
Codebuch Stand 2025-01
erstellt von Team Ocean Race (Ansprechpartnerin Viktoria Reiser vr047@hdm-stuttgart.de)

## Inhalt
- Edgelist_OceanRace.csv (Edgelist)
- Nodelist_OceanRace.csv (Nodelist)
- OceanRace.rmd (Markdown-Dokument)
- Codebuch.md (Codierung der Datensätze)
- Zeiterfassung_Projekt.md (Zeitplan)

## Ursprung und Datenerhebung
Wir haben einen Datensatz für den Pretest eines Netzwerks von "the Ocean Race" aus den Episoden 2014/15 und 2017/18 erhoben. Die Daten haben wir auf der offiziellen Webseite von Ocean Race, den entsprechenden Wikipedia-Artikeln und einzelnen Webseiten zu den Teams gefunden. 

Das Netzwerk ist ein *gerichtetes three-mode Netzwerk*, das sich in zwei Arten von Netzwerke gliedern lässt. 

1) Ein Zusammenarbeitsnetzwerk *team*, das die Verbindung aller Segler aus den Jahren 14/15 und 17/18 zu ihren Teams darstellt.

2) Ein Nationalitätennetzwerk *nationality*, das die Verbindung aller Segler zu ihrer Nationalität darstellt.

**Umgang mit fehlenden Werten:**
Fehlende Werte werden nicht erfasst.

# EDGE-Attribute

**from** <br>
initiierender Knoten, in diesem Fall: Segler

**to** <br>
erhaltender Knoten, in diesem Fall: Team, in dem der Segler angetreten ist 

**position** <br>
crew = crew member <br>
skipper = skipper im Team


# NODE-Attribute  
  
**id** <br>   
Alphanumerisch: Initialen des Seglers (bei Dopplung wurde bei einem der Segler der zweite Buchstabe des Nachnamens ergänzt), als string/characters codiert 

**sailor** <br>
Alphanumerisch: Voller Name des Seglers, als string/characters codiert

**nationality** <br>

AUS - Australien <br>
AUT - Österreich <br>
ARE - Vereinigte Arabische Emirate <br>
ARG - Argentinien <br>
BEL - Belgien <br>
BM - Bermuda <br>
BR - Brasilien <br>
CH - Schweiz <br>
CHN - China <br>
DNK - Dänemark <br>
ESP - Spanien <br>
FIN - Finnland <br>
FRA - Frankreich <br>
GER - Deutschland <br>
IR - Irland <br>
IT - Italien <br>
NLD - Niederlande <br>
NOR - Norwegen <br>
NZ - Neuseeland <br>
PG - Papua-Neuguinea <br>
PT - Portugal <br>
RUS - Russland <br>
SE - Schweden <br>
UK - Vereinigtes Königreich <br>
UKR - Ukraine <br>
US - Vereinigte Staaten von Amerika <br>
ZAF - Südafrika <br>

**sex** <br>
1 = männlich <br>
2 = weiblich <br>

**type** <br>
1 = Segler <br>
2 = Teams <br>

##
