# Lern-Periode-10
## 21/02/2025
### Arbeitspakete
- [x] Mit Cezar C# repetiert
- [x] M426 SCRUM repetition
- [x] M426 OBA vorbereitung

#### Gelerntes
(Heute eher repetiertes)
- Variable scoping C#
- SCRUM
  - SCRUM master, product owner, dev team
  - Inkrement
  - Prozess
  - Stand-ups, Retrospectives, Review, Planning
  - Sprint

#### Notiz
Ich denke scrum ist eine gute Methode um software zu entwickeln, aber das Projekt benötigt eine gewisse grösse damit es sich überhaupt lohnt. Schwierigkeiten hatte ich heute nur dabei zu erkenne, dass ein Fehler im Code an Variable Scoping lag, aber ansonsten lief alles gut.

## 09/05/2025
### Arbeitspakete
- [x] Python ML repetiert
- [x] OSU! Beatmap dataset gesucht und geladen
- [x] OSU! beatmap syntax analysiert und docs gelesen

#### Notiz
Aktuelles Projektziel: OSU! bot mit ML

## 16/05/2025
### Arbeitspakete
- [x] Lösungansätze Modeltraining suchen (generation Trainingsdaten (Ja, das dauerte wirklich so lange))
  - [x] script mockup
  - [x] Script abstimmen mit custom in-game skin
  - [ ] script logik, render, usw.

### Notiz
⠀⠀⠀⡄⠀⢠⡄⠀⠀⣤⠀⢠⡄⠀⢠⣤⠀⢠⡄⠀⢠⡄⠀⢠⣤⠀⢠⡄⠀⠀<br>
⠀⠀⠀⡇⠀⢸⡇⠀⠀⣿⠀⢸⡇⠀⢸⣿⠀⢸⡇⠀⢸⡇⠀⢸⣿⠀⢸⡇⠀⠀<br>
⠀⠀⠀⡇⠀⢸⡇⠀⠀⣿⠀⢸⡇⠀⢸⣿⠀⢸⡇⠀⢸⡇⠀⢸⣿⠀⢸⡇⠀⠀<br>
⠀⠀⠀⡇⠀⢸⡇⠀⠀⣿⠀⢸⡇⠀⢸⣿⠀⢸⡇⠀⢸⡇⠀⢸⣿⠀⢸⡇⠀⠀<br>
⠀⠀⠀⡇⠀⢸⡇⠀⠀⣿⠀⢸⡇⠀⢸⣿⠀⢸⡇⠀⢸⡇⠀⢸⣿⠀⢸⡇⠀⠀<br>
⠀⠀⠀⡇⠀⢸⡇⠀⠀⣿⠀⢸⡇⠀⢸⣿⠀⢸⡇⠀⢸⡇⠀⠸⠿⠀⠸⠇⠀⠀<br>
⠀⠀⠀⡇⠀⢸⡇⠀⠀⣿⠀⢸⡇⠀⠸⠿⠀⠘⠃⠀⠸⠇⠀⣠⣴⣶⣶⣄⠀⠀<br>
⠀⠀⠀⡇⠀⢸⡇⠀⠀⣿⠀⠘⠁⣀⣤⣶⣶⣾⣿⣷⣶⣤⣾⣿⣿⣿⣿⣿⠀⠀<br>
⠀⠀⠀⡇⠀⢸⡇⠀⠀⠋⣠⣶⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⠃⠀⠀<br>
⠀⠀⠀⡇⠀⢸⡇⠀⠀⣼⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⡝⠻⠿⠟⠋⠁⠀⠀⠀<br>
⠀⠀⠀⡇⠀⢸⡇⠀⢸⣿⣿⣿⣿⣿⠟⠛⠉⠁⠹⣿⣿⣇⠀⠀⠀⠀⠀⠀⠀⠀<br>
⠀⠀⠀⡇⠀⢸⡇⠀⠘⣿⣿⣿⣯⠀⠀⠀⠀⠀⠀⢿⣿⣿⡄⠀⠀⠀⠀⠀⠀⠀<br>
⠀⠀⠀⡇⠀⠘⠃⠀⠀⠘⠿⣿⣿⣷⣄⠀⠀⠀⠀⠈⢿⣿⣿⡄⠀⠀⠀⠀⠀⠀<br>
⠀⠀⠀⢠⣶⣶⣶⣶⣶⣶⣾⣿⣿⣿⣿⣷⣄⠀⠀⠀⠈⢿⣿⣿⣆⠀⠀⠀⠀⠀<br>
⠀⠀⠀⠛⠛⠛⠛⠛⠛⠛⠛⠛⠛⠛⠛⠛⠛⠓⠀⠀⠀⠀⠙⠛⠛⠓<br>
"Why?"

Also: Heute habe ich herausgefunden, dass ich mehrere Stunden Nachforschung, das Lesen von Dokumentationen und Scripting verschwendet habe. (Natürlich erst am Schluss, wie es sich gehört.)

Mein grösstes Problem bei diesem Projekt war (ist) das Erstellen der Trainingsdaten. Mein Plan ist es, das Modell über einen herunterskalierten Video-Feed laufen zu lassen. Das wäre der X-Trainingsdatensatz. Y wären Mauskoordinaten und Mouse_Keydown (1, 0). Um den Videofeed zu generieren, wollte ich ein Script schreiben, welches eine .osu-Map-Datei einliest und diese in ein Video umwandelt.

Jetzt hat sich aber herausgestellt, dass der neue Osu!-Client (Osu!-Lazer) einen Headless-Mode zur Verfügung stellt. (=____=)

Das bedeutet, ich muss nur eine perfekte Replay-Datei (.osr) erstellen, die Map-Datei nehmen und beides an Osu! per Kommandozeile weitergeben, welches es dann in eine Videodatei umwandelt.  
Ich bin gleichzeitig erleichtert (mein Script funktioniert nämlich nicht) und einfach nur fertig mit diesem ganzen Projekt, da ich so viel Zeit und Mühe verschwendet habe.

Naja, jetzt sollte es wenigstens wieder ein wenig schneller vorwärtsgehen.

[Osu!](https://osu.ppy.sh/)  
[Osu!Lazer (Source)](https://github.com/ppy/osu)  
[.osu](https://osu.ppy.sh/wiki/en/Client/File_formats/osu_%28file_format%29)  
[.osr](https://osu.ppy.sh/wiki/en/Client/File_formats/osr_%28file_format%29)

## 23/05/2025
### Arbeitspakete
- [x] Osu! ML-optimierter skin fertigstellen
- [x] Osu! Video von Map-Datei erstellen
- [ ] Osu! replay von Map-Datei erstellen

### Notiz
Der Skin funktioniert jetzt, ich habe es geschaft mit [danser](https://github.com/Wieku/danser-go) ein video eines perfekten Replays von einer Map zu erstellen.<br>
Das nächste Mal experimentiere ich noch mit dem Osu-headless mode. Ich habe heute Danser verwendet, da es einiges leichter ist als der ganze osu-client und deshalb hoffentlich auch schneller, aber die Erstellung von Videos ist langsam (weiss nicht ob headless besser ist) und es ignoriert einige meiner Einstellungen. Zudem, wie ich nun herausgefunden habe, unterstützt es den Export der Replay-Daten nicht und das Video allein ist eher nutzlos.<br>
Osu headless sollte all das hoffentlich unterstützen und dann könnte ich vielleicht bald mit dem Training anfangen.<br>
Ich habe realisiert: Datenaufbereitung ist genau so mühsam wie Modeltraining, wenn nicht sogar mehr.

## 07/06/2025
### Arbeitspakete
- [x] LB254 HZ1.1 Korrigieren
- [x] LB254 HZ3.1 Machen
- [x] LB254 HZ3.2 Machen

### Notiz
Heute habe ich an der LB254 gearbeitet, da wir momentan viele Prüfungen haben und ich deshalb froh bin wenn ein wenig dieser Arbeitslast im Lernatelier ablegen kann um auch noch für die Kanti-Fächer zu lernen. Das Modul 254 ist ein wenig trocken mit viel Theorie, aber ich denke ich habe es verstanden und es scheint nicht sehr kompliziert. (Mindestens die Grundlagen)
