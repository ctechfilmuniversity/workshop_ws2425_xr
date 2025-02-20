# Towar

## Projektübersicht

TOWAR verwandelt selbstgebaute Festungen in lebendige Verteidigungsanlagen: Ob Sandburg am Strand, Kissenfort im Wohnzimmer oder Kartenburg auf dem Tisch – mit AR-Technologie wird jede Konstruktion zum interaktiven Spielfeld. In dieser Verschmelzung von echter und digitaler Welt verstecken Spieler einen virtuellen Schatz in ihrer selbstgebauten Festung und verteidigen ihn gegen anrückende Gegner. Mit dem Smartphone als Bogen bewaffnet, gilt es die eigene Kreation zu beschützen und die Angreifer in die Flucht zu schlagen.

## Spielmechanik

### Grundkonzept

- Spieler errichten eine physische Verteidigungsanlage (z.B. eine Sandburg) in der realen Welt
- Ein virtueller Schatz wird innerhalb der Verteidigungsanlage platziert
- Virtuelle Gegner versuchen den Schatz zu erobern
- Der Spieler verteidigt den Schatz mit AR-Bogenschießen

### Verteidigungssystem

- Das Smartphone fungiert als virtueller Bogen
- Spieler können Pfeile aus der Kameraperspektive abfeuern
- Gegner werden nach drei Treffern eliminiert

### Spielziele

- **Sieg**: Eliminierung aller Angreifer vor Verlust des Schatzes
- **Niederlage**: Ein Angreifer erreicht den Schatz

## Technische Implementierung

### AR-Scanning

- Nutzung des ARKit-Frameworks für Umgebungserfassung
- Erstellung eines navigierbaren Mesh der Spielumgebung
- Integration physischer Strukturen in die Spielmechanik

### Gegner-KI

- Dynamische Wegfindung über das gescannte Mesh
- Zielgerichtete Bewegung zum Schatz
- Definierter Auslöseradius für Spielende

## Spielablauf

1. **Vorbereitungsphase**
   - Umgebungsscanning durch den Spieler
   - Platzierung des virtuellen Schatzes
2. **Spielphase**
   - Spawn der Gegner in definiertem Abstand zum Schatz
   - Bewegung der Gegner über das Mesh
   - Aktive Verteidigung durch den Spieler
3. **Spielende**
   - Siegbedingung: Elimination aller Gegner
   - Verlustbedingung: Schatz wird erreicht
