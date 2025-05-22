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
[Osu!Lazer GitHub](https://github.com/ppy/osu)  
[.osu](https://osu.ppy.sh/wiki/en/Client/File_formats/osu_%28file_format%29)  
[.osr](https://osu.ppy.sh/wiki/en/Client/File_formats/osr_%28file_format%29)
