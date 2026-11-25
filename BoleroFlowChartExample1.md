# Berekening meerwaardebelasting, Bolero example 1

> *Voorbeeld 1*
>
> *Je kocht in 2023 verschillende keren hetzelfde aandeel aan een gemiddelde aankoopkoers (GAK) van €150. De slotkoers op 31 december 2025 bedraagt €120. Je verkoopt later het volledige pakket aan €125. Omdat de GAK (€150) hoger ligt dan de waarde op het startpunt (€120), wordt de GAK gebruikt als aanschaffingswaarde. Er ontstaat geen meerwaarde aangezien de verkoopprijs (€125) lager ligt dan de GAK (€150). Daarom is geen meerwaardebelasting verschuldigd.*
>
> *Bron: https://www.bolero.be/nl/lp/meerwaardebelasting*

---

```mermaid
flowchart TD

    A["Aankopen in 2023<br/>Gemiddelde aankoopkoers (GAK) = €150"]

    B["Slotkoers op 31-12-2025<br/>= €120"]

    C{"Is GAK hoger<br/>dan startpunt?"}

    D["Gebruik GAK<br/>als aanschaffingswaarde"]

    E["Gebruik startpunt<br/>als aanschaffingswaarde"]

    F["Verkoopprijs = €125"]

    G["Bereken meerwaarde"]

    H{"Meerwaarde > 0 ?"}

    I["10% meerwaardebelasting"]

    J["Geen meerwaardebelasting"]

    A --> C
    B --> C

    C -->|Ja| D
    C -->|Nee| E

    D --> F
    E --> F

    F --> G
    G --> H

    H -->|Ja| I
    H -->|Nee| J
```
