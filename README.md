# HutschienenShild-D1-mini
Wemos D1 direkt in Verteilung incl. Spannungsversorgung 5V nutzen

Nach dem die App von meinem Energieversorger versagte, wollte ich meinen Haupt- und Zwischenzähler per S0 bzw. D0 auslesen können und die Daten Speicher können.
Bei Youtube konnte ich dann erfahren, wie die Daten auf einen Raspberry gespeichert, ausgewertet und angezeigt werden können. Was fehlte war die Möglichkeit einen ESP8266 direkt auf die Hutschiene zu setzten und nur noch anzuschießen.
Darum habe ich mich rangesetzt, ein Shield zu entwikeln.

# Schaltplan:
![](https://github.com/Elektrofix-OL/HutschienenShild-D1-mini/blob/main/Eagle/sch.GIF)
Wie zu sehen ist, ist das ganze nicht's besonderes. Aus 230V-AC werden über ein Wandler 5V-DC bereitgestellt. Der D1-Mini macht daraus seinen 3,3V und die Ein-/Ausgänge werden direkt an SV1 herausgeführt.
Auf der Leiterplatte sind für die Anschlüsse SV1-7 bis SV1-9 Pullup- und Pulldown-Widerstände möglich, wobei dort natürlich auch einen Freilaufdiode eingelötet werden können.
Auf der Unterseite sind Lötbrücken vorgesehen. So kann jeder selber entscheiden, welcher GPio von nutzen ist, da einige GPio's beim Booten des D1-Mini eine bestimmten Pegel haben müssen. Mit diesen Brücken können somit 5 digitale, oder 4 digitale und der analogen GPio's genutzt werden.
Am SV1 sind außer die 5 GPio-Zugänge noch Tx, Rx, +5V, +3,3V und GND erausgeführt. Ferne ist es möglich noch im Gehäuse ein weiteres Shild unterzubringen (sieh Foto's) 

# Gehäuse-Bilder
![](https://github.com/Elektrofix-OL/HutschienenShild-D1-mini/blob/main/Foto/Seitenansicht.jpg)
![](https://github.com/Elektrofix-OL/HutschienenShild-D1-mini/blob/main/Foto/Seitenansicht_mit%20Wemos.jpg)
![](https://github.com/Elektrofix-OL/HutschienenShild-D1-mini/blob/main/Foto/Seitenansicht_ohne_Wemos.jpg)
Wie zu sehen ist, passen die Kontakthalten nicht ganz, daher haben ich mit einem Cutter die beinden letzten Kontakthalter halbiert. Der elekrische Kontakt wird nicht beeinträchtigt.
Der Kondensator kann auch größer gewählt werden, bei mir dient er als Glättung, damit die Schaltung nicht ins Schwingen kommt.

# Bauteile
für die Bauteile habe ich eine Liste bei [www.reichelt.de](https://www.reichelt.de/my/1790195) erstellt. 
