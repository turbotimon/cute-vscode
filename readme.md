# CUTE mit vscode

## vsCode Extension
- *C/C++* extension installieren
- (*Code Runner* extension installieren. Weiss nicht ob nötig für das, aber funktioniert gut für einzelne cpp-files um kurz was zu testen)
- *CMake* extension installieren

## Projektstruktur gleich wie bei clion
- CMakeLists.txt im Hauptordner
- Unterordner `cute` für Cute Files und `src` für alles andere (eure Code)

## CMakeLists.txt anpassen
- Die mit `--> .. <--` markierten Orte müssen eventuell auf eure Projekt und eure Installation angepasst werden.

## Projekt kompillieren und laufen lassen
- Rechtsklick auf Hauptordner und *in Visuals Studio Code* öffnen 
- Bei öffnen kommt ev eine Meldung *wollen sie cmake konfigurieren*, das gemacht (irgendwas mit *kit* und *variant*) wo dec g++-Kompiler ausgewählt werden sollte. Danach wurde der `build` ordner erstellt. Kompiler kann sonst auch nachher in der Taskleiste gewechselt werden.
- In der Taskleiste gibt es ein **Cmake: [DEBUG]: Ready** für die Konfig. Dort kann zwischen Debug und Release gewechselt werden
- In der Taskleiste auf **Build [all]** klicken. Danach auf **Run** klicken. Sollte laufen in der Konsole laufen..

## Hilfe
- https://code.visualstudio.com/docs/cpp/cmake-linux
