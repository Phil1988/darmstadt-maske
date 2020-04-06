# Darmstadt-Maske: Gesichtsmasken für hub-rheinmain und hub-darmstadt

Warum denn "noch eine Maske"? 
Gute Frage - wir haben nach etlichen Erfahrungswerten festgestellt, dass die Prusa-Masken zwar sinnvoll sind und sich das Maß für die Visiere etabliert hat, aber einige Interessenten fragten nach einer größeren Entfernung zwischen Gesicht und Visier oder der Möglichkeit auch andere besser desinfizierbare Kopfbänder zu befestigen.
Außerdem wurde bei unserem Modell die Druckzeit durch Konstruktive veränderungen deutlich reduziert (bis zu 40% schneller).
Dieses Modell ist jedoch weiterhin vollständig kompatibel zur Prusa-Variante.

Als groben Richtwert, kann man das Kopfteil in etwa 60min drucken - mit einer 0.4mm Düse.
Wer deutlich länger benötigt, sollte sich nochmal alle Informationen, die wir hier zusammentragen, anschauen oder mit uns in Kontakt treten.

## Disclaimer

Diese Gesichtsmasken sind kein medizinisches Produkt, sind nicht zertifiziert und eine Herstellung und Benutzung geschieht auf eigene Gefahr. Jegliche Haftung ist ausgeschlossen.

## Qualitätsicherung

Wir freuen uns über jeden der der sich uns anschließt und wir gemeinsam noch besser helfen zu können.
Bitte denkt daran, dass man mit dieser herstellung dieser Maske eine gewisse Verantwortung hat.
Daher überprüft bitte selbst die Qualität eurer Drucke.

Diese wird zwar beim Zusammenbau auch nochmal überprüft, aber es erspart uns und euch Zeit und schont die Umwelt, wenn alle Modelle eine gute Qualität aufweisen.

Hier ein Video das zeigt, welche mechanischer Belastung die Maske aushält:
[Youtube-Video](https://youtu.be/hdetuEkw_Qs )

Solltet ihr Probleme haben, dann lest zuerst bitte alle Hinweise auf dieser Seite durch und fragt uns danach um Hilfe für die passenden Druckeinstellungen.

## Credits

Dieses Repository ist maßgeblich beinflusst von https://github.com/yschroeder/face-shield.

## TL;DR

* Nutzt `PrusaSlicer` und stellt den in den Experten-Modus (rechts oben).
* Alle Geschwindigkeiten auf die Geschwindigkeit `Eilgang` (`Travel Speed`) stellen, außer `Stützstrukturen` (`Support Material`), `Überbrückungen` (`Bridges`), `Lückenfüllung` (`Gap Fill`) und `Druckgeschwindigkeit der ersten Schicht` (`First layer speed`). Die echte Druckgeschwindigkeit wird ohnehin durch den maximalen Material Durchsatz eures Extruders begrenzt, sodass der Drucker die eingegebenen Geschwindigkeiten nicht erreichen wird.
* Setzt die in eurem Filament die Maximale Volumengeschwindigkeit (`Max. Volumetric Speed`) auf 8mm³/s. Das könnt ihr erhöhen bis der Druck unsauber wird. Geeignet sind 2mm³/s Stufen. Sollte es zu lauten Knackgeräuschen aus dem Extruder kommen, ist der Wert zu hoch.
* Setzt das Infill auf auf 10% und nehmt Gyroid. Das druckt minimal langsamer als ohne Infill, sollte dadurch aber stabiler sein.
* Die Extrusionsbreite ist abhängig von eurem Drucker. Sollten sich zwischen den Hüllen Abstände befinden, ändert die Extrusionsbreite `Konturen` (`Perimeter`) und `Außenkonturen` (`External Perimeter`) auf etwas breiter, z.B. 0.48mm

## FAQ

Q: Warum druckt ihr eigene Designs? Es gibt doch schon so viele!

A: Das ist richtig, wir haben uns allerdings entschieden ein etwas anderes Design als bspw. Prusa zu verwenden, um eine in unseren Augen bessere Balance zwischen Druckzeit, Stabilität und Tragekomfort zu erreichen. Weiterhin ist die darmstadt-maske vollständig kompatibel zu den bei Prusa genutzten Knopfloch-Gummi-Bändern und den Visieren. Der hervorstechendste Unterschied ist ein größerer Abstand zwischen dem Gesicht und dem Visier. Außerdem kann das Modell, durch eine für die meisten 3D Drucker besser optimiertes Design, vergleichsweise schnell gedruckt werden.


Q: Ist euer Design denn stabil genug?

A: Wir sind der Ansicht, dass es keine Einschränkungen hinsichtlich der Stabilität geben sollte, auch wenn die Maske mit großen, schweren Folien (zB 0,8mm PETG) ausgestattet wird.

Q: Ich nutze Cura. Gibt es dafür auch ein Einstellungs-Set?

A: Aktuell nicht. Sollten wir erhöhten Bedarf sehen, könnte sich das aber ändern. Der PrusaSlicer in Version 2.2 unterstützt übrigens inzwischen auch den die Drucker der Ender 3 Serie. Vielleicht ist das eine Chance einen Blick drauf zu werfen.

## Modelle

In diesem Repository findet man im Ordner stl das aktuelle Modell.
Hier eine kleine Übersicht.
Sollten dort in Zukunft mehr Versionen dazukommen, wird diese Übersicht ergänzt.

### stl/Darmstadt_Maske_v2_ohne_pad.stl
Das einfache Modell. Simpel, gut zu drucken und gut, um Druckeinstellungen zu testen.

### stl/Darmstadt_Maske_v2_mit_pad.stl
Im Vergleich zum Modell "ohne Pad" ist hier an den Enden des Kopfteils rechts und links ein kleines "Pad" dazugekommen.
Auf dem folgenden Bild grün markiert:

![Veranschaulichung Pad](https://raw.githubusercontent.com/Phil1988/darmstadt-maske/master/pad.PNG)

Dieses Modell erhöht an diesen Stellen die Haftung und ist für Leute zu empfehlen, die dort Probleme haben.
Das Pad lässt sich nach dem Druck einfach mit einem Seitenschneider entfernen und liegt auf der Außenseite, damit die beim Abschnitt entstehenden scharfen Kanten nicht unangenehm an der Stirn sind.


### stl/Darmstadt_Maske_v2_Xer_Stapel_mit/ohne_pad.stl
Dies sind gestapelte Modelle mit und ohne "Pad".
Durch die Stapelung, kann mehrere Modelle (z.B. über Nacht) an einem Stück drucken.
Leider fällt hierdurch aber ein zusätzlicher Arbeitsschritt an, da man die Modelle an den Sollbruchstellen erst lösen muss.
 
 
## Erklärung zu Druckeinstellungen

Wichtig ist, dass ihr beachtet, dass euer Drucker Grenzen hat, die wir nicht kennen.
Alle hier genannten Werte für die Geschwindigkeit sind Richtwerte für unsere Drucker.
Im Zweifel solltet ihr euch lieber erstmal an diese Werte ran tasten

Die Druckgeschwindigkeit wird maßgeblich von der Förderrate oder der `Maximalen Volumengeschwindigkeit` (`Max. Volumetric Speed`) beeinflusst. Das Modell ist simpel und hat ein gewisses Volumen, das durch den Druckkopf gedrückt werden muss. Ist diese Fördermenge kleiner, dauert der Druck länger. Angegeben wird diese in mm³/s. Richtwert für PLA ist etwa 10-12mm³/s.
Um die Fließeigenschaften des Kunststoffes zu verbessern, kann es ratsam sein, die Temperatur um 5-10°C höher zu stellen.

Als Schichthöhe drucken wir größtenteils mit 0,3mm.

Weiterhin möchte man Dinge vermeiden, die den Druckkopf bremsen. Dazu gehört langsam gedruckte Lückenfüllungen (`Gap fill`), Infill und andere enge Radien, bei denen der Drucker langsam fahren muss.

Als Beispiel hier ein Bild, mit dunkelrotem Infill und weißer Lückenfüllung, die beide sehr eng langsam gedruckt werden.
![Gap Fill and Infill][gap_infill]

Dieses Beispiel zeigt ein Bild eines Objekts, was nur aus einer Hülle besteht und daher sehr schnell zu drucken.
![Only Perimeters][perimeter]

Um schnell druckbare Objekte zu bekommen, muss man in der Regel beim Design ansetzen. Bei dem Modell der Darmstadt-Maske wurde darauf geachtet, die gängige Wandstärke von 1.67mm einzuhalten, um eine glatte Anzahl gängiger Spurbreiten zu erhalten und so auf Lückenfüllungen zu verzichten. Deswegen ist die Einstellung der richtigen Extrusionsbreite entscheidend. 
Für eine 0.4mm Düse, ist eine Bahnbreite von 0.48mm ein guter Startwert. Man sollte aber beim Slicen selbst die Bahnen prüfen und die Breite entsprechend anpassen.

Da letzten Endes nur die maximal mögliche Volumengeschwindigkeit relevant ist, kann der Drucker also in allen anderen Geschwindigkeiten auf seine maximale Geschwindigkeit eingestellt werden (z.B. 100mm/s). Hier eignet sich der Wert der unter `Eilgang` (`Travel Speed`) eingetragen ist. Wichtig: Sollten gestapelte Versionen gedruckt werden, so ist wichtig, dass der Haken bei `Umfangbrücken entdecken` (`Detect bridging Perimeters`) gesetzt und die Geschwindigkeit von Brücken auf einen sehr niedrigen Wert gesetzt ist. Sinnig sind hier ca. 30-50mm/s. Das erleichtert später den Prozess des Zerlegens. Die Geschwindigkeit für Lückenfüllungen sollte auf 0 gesetzt werden, um diese ganz zu vermeiden.

Anschließend kann der Gcode aus dem Modell generiert werden. Die Druckdauer sollte sich nicht nennenswert oberhalb einer Stunde pro Maske befinden. Wenn doch, bitte unten in der Rubrik Troublshooting nachschauen oder mit uns in Verbindung setzen (z.B. slack, telegram, hier ein issue eröffnen, etc.).

## Troubleshooting

Problem: Ich kann zwischen Bahnen durchgucken oder sie halten nicht aneinander.

Lösung: Wenn die Bahnen so auseinander stehen, dass man gewissermaßen von oben das Druckbett durch das Teil sehen kann, dann solltest du versuchen, ob sich das Ergebnis mit leicht breiteren Bahnen beheben lässt. Beispielsweise 0.48mm Bahnbreite oder noch etwas mehr verwenden. Wenn sich seitlich durch den Druck gucken lässt oder sich die einzelnen Schichten voneinander ablösen, dann scheinst du zu wenig Material zu verdrucken. Das kann mehrere Gründe haben, lässt sich aber vermutlich am einfachsten durch einen höheren Extrusionsmultiplikator lösen. Eventuell ist eine geringere Schichtdicke sinvoll.

[gap_infill]: gap_infill.PNG "Infill und Lückenfüllungen"

[perimeter]: perimeter.PNG "Nur Hüllen"
