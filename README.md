# ha-ir-sauna

This Home Assistant blueprint controls two infrared heaters (`strahler_liege` and `strahler_oben`). It offers four operating modes:

- **AUS**: Turns both heaters off.
- **Gleichmässig**: Runs both heaters at a constant brightness for the configured duration.
- **Intervall**: Ramps brightness up and down in steps for a wave-like effect, repeating until the overall timer expires.
- **Einmal AUF und AB**: Performs a single up-and-down brightness cycle over the total duration.

Duration, maximum intensity, and cycle length (for *Intervall*) are taken from `input_number` helpers. A Home Assistant `timer` tracks the remaining runtime and stops the program when it finishes or is cancelled.
