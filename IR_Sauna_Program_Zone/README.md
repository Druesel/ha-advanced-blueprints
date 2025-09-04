# IR Sauna – Programm Zone

Dieser Blueprint steuert zwei Infrarot-Strahler einer IR-Liege. 
Über ein `input_select` lässt sich eines von vier Programmen wählen:

- **AUS** – schaltet beide Strahler aus
- **Gleichmässig** – beide Strahler laufen für die gewählte Dauer mit konstanter Intensität
- **Intervall** – beide Strahler fahren wellenförmig rauf und runter; Dauer eines Zyklus kommt aus einem Helper
- **Einmal AUF und AB** – einmaliger Zyklus von Minimum zu Maximum und wieder zurück

Zusätzlich werden folgende Helper benötigt:

- `input_number` für Programmdauer in Minuten
- `input_number` für maximale Intensität in Prozent
- `input_number` für die Zyklusdauer des Intervall-Programms
- `timer` zur Anzeige der Restlaufzeit
- `light` Entitäten für die Strahler „Liege" und „Oben"

Weitere Details und Anpassungen können direkt im YAML Blueprint vorgenommen werden.
