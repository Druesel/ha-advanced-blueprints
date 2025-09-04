# IR Sauna – Programm Zone

Dieser Blueprint steuert zwei Infrarot-Strahler (Liege und Oben) einer IR-Liege mit verschiedenen Programmen.

## Funktionen
- **AUS**: Beide Strahler werden ausgeschaltet.
- **Gleichmässig**: Beide Strahler laufen für die gewählte Dauer mit einer konstanten Intensität.
- **Intervall (Welle)**: Die Intensität beider Strahler steigt und fällt gleichlaufend in einem wiederholten Zyklus.
- **Einmal AUF und AB**: Ein einzelner Zyklus, bei dem die Intensität einmal von Minimum zu Maximum und wieder zurück fährt.

Die Programmdauer, die maximale Intensität und die Zyklusdauer lassen sich über Helpers konfigurieren. Ein Timer zeigt die Restlaufzeit im Dashboard an.
