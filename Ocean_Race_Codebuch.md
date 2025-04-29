# Datensatz Ocean Race #
Codebuch Stand 2025-04-29
erstellt von Team Ocean Race 
Ansprechpartner: Viktoria Reiser vr047@hdm-stuttgart.de

## Inhalt
- Edgelist_OceanRace.csv (Edgelist)
- Nodelist_OceanRace.csv (Nodelist)
- OceanRace.rmd (Markdown-Dokument)
- Codebuch.md (Codierung der Datensätze)
- Zeiterfassung_Projekt.md (Zeitplan)

## Ursprung
Für den Pretest haben wir einen Datensatz der Teilnehmern des Ocean Race aus den Jahreb 2014/15 und 2017/18 erhoben. Die Daten haben wir auf der offiziellen Webseite von Ocean
Race, den entsprechenden Wikipedia-Artikeln und einzelnen Webseiten zu den Teams gefunden. Hauptzugang war über Teilnehmerlisten.

Das Netzwerk ist ein *gerichtetes three-mode Netzwerk*, das sich in zwei Arten von Netzwerken gliedern lässt. 
1) Ein Zusammenarbeitsnetzwerk *team*, das die Verbindung aller Segler aus den Jahren 14/15 und 17/18 zu ihren Teams darstellt.
2) Ein Nationalitätennetzwerk *nationality*, das die Verbindung aller Segler zu ihrer Nationalität darstellt.

## Finale Erhebung 

Auf Basis des Pretest und wissenschaftlicher Lektüre hat sich folgende Forschungsfrage für das Ocean Race Netzwerk ergeben: Was sagt die Netzwerkstruktur der Teams von The Ocean Race (08/09–22/23) über die Zusammenarbeit der Sportler und den Einfluss ihres kulturellen Hintergrunds auf diese aus?
Vorhandene Daten wurden über offizielle Teilnehmerlisten, Wikipedia Einträge und erweiterte Recherche über die Sozialen Medien und die Presse erhoben.

**Umgang mit fehlenden Werten:**
Fehlende Werte werden nicht erfasst.

# EDGE-Attribute
**from** <br>
initiierender Knoten, in diesem Fall: Segler

**to** <br>
erhaltender Knoten, in diesem Fall: Team, in dem der Segler angetreten ist 

**position** <br>
crew = Crew Member <br>
skipper = Skipper im Team


# NODE-Attribute  
**id** <br>
Die id besteht aus den Initialien des Seglers (= Anfangsbuchstabe Vorname + Anfangsbuchstabe Nachname). Bei Dopplungen der ids wurde der zweite Buchstabe des Nachnamens des Seglers ergänzt.
Codierung: alphanumerisch, als string/characters

**sailor** <br>
Dieses Attribut steht für den vollen, ausgeschriebenen Namen des Seglers.
Codierung: alphanumerisch, als string/characters

**nationality** <br>
Das Attribut "nationality" steht für die internationale Ländercodes des jeweiligen Landes.

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
Mit diesem Attribut wurde das Geschlecht der Segler erhoben. In der Erhebung wurde zwischen männlich, weiblich und divers unterschieden. Allerdings wurden nur Teilnehmer erfasst, die sich als männlich oder weiblich identifizieren, weshalb nur zwischen zwei Geschlechtern unterschieden wird.
1 = männlich <br>
2 = weiblich <br>

**position** <br>
Hier wird gezeigt, in welcher Position der Segler in dem Rennen teilgenommen hat. Dabei hat sich das Forschungsteam auf die Unterscheidung zwischen Skipper und Crew Member entschieden, da eine genauere Aufschlüsselung zu komplex für die vorliegende Netzwerkanalyse ist.
1 = als Skipper teilgenommen <br>
2 = als Crew Member teilgenommen <br>

**type** <br>
Mit diesem Attribut wurden Knoten als Segler oder Team codiert. In Visualisierungen konnten so unterschiedliche Formen/Farben für die jeweiligen Knoten angewendet werden.
1 = Segler <br>
2 = Teams <br>

**winner** <br>
Jede Saison steht am Ende des Ocean Race auch ein Gewinner fest. Wer gewonnen oder verloren hat, wurde mit diesem Code festgelegt.
1 = winner <br>
2 = loser <br>

**homogenity** <br>
Die Homogenität von Teams bezieht sich auf die Kulturdimensionen nach Hofstede. Als homogen werden Teams eingestuft, die mehr als zweidrittel (>66%) an Teammitgliedern vorweisen, die demselben Kulturquadranten zugeordnet werden.
1 = homogen <br>
2 = heterogen <br>
##
