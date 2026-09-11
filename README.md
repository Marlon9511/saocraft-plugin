# SaoCraft

Ein Sword-Art-Online-inspiriertes Spigot-Plugin für Minecraft. Es nutzt nur eigene
Mechaniken, Farben und Item-Namen – keine Original-Grafiken, Logos oder Texte aus
dem Anime/den Spielen.

## Features

- **Sword Skills**: Schleichen + Rechtsklick mit einem Schwert löst deinen aktuell
  ausgerüsteten Skill aus (Horizontal, Vertical, Sonic Leap, Starburst Stream),
  jeweils mit eigenem Cooldown, Bonus-Schaden, Partikeln und Sound.
- **HP-Balken über dem Kopf**: Jeder Spieler bekommt einen für alle sichtbaren
  Lebensbalken über dem Kopf, der sich live mit der Farbe grün/gelb/rot ändert.
- **Duell-System**: `/duel <spieler>` fordert heraus, `/duel accept` nimmt an.
  Sobald die HP eines Duellanten auf 0 fallen würde, wird das als Niederlage
  gewertet, kein echter Tod – beide werden geheilt und zurückteleportiert.
- **Status-Menü**: `/saomenu` öffnet ein Inventar-GUI im SAO-Stil mit HP, Level,
  ausgerüstetem Skill, allen verfügbaren Skills und Duell-Status.

## Befehle

| Befehl | Beschreibung |
|---|---|
| `/skill list` | Zeigt alle Sword Skills |
| `/skill <horizontal\|vertical\|sonicleap\|starburst>` | Skill ausrüsten |
| `/duel <spieler>` | Duell anfragen |
| `/duel accept` / `/duel decline` / `/duel leave` | Anfrage annehmen/ablehnen/Duell verlassen |
| `/saomenu` (Alias `/status`) | Status-Menü öffnen |

## Bauen

Voraussetzung: Java 17+ und Maven.

```bash
mvn clean package