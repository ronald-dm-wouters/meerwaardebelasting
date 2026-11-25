# Berekening meerwaardebelasting, Bolero example 2

<sub><i>
Voorbeeld 2: aankoop vóór 31-12-2025, GAK is lager dan de slotkoers van 31-12-2025 en de verkoop gebeurt boven de GAK.
Je kocht een aandeel in verschillende stappen vóór 2026: in 2023 aan €100 en in 2024 aan €140, waardoor de gemiddelde aankoopprijs (GAK) €120 bedraagt.
De slotkoers op 31 december 2025 bedraagt €130 (het startpunt).
Je verkoopt het volledige pakket in 2028 aan €150.
Omdat de GAK (€120) lager ligt dan de waarde van het aandeel op het startpunt (€130), wordt het startpunt gebruikt als aanschaffingswaarde.
De belastbare meerwaarde bedraagt €20 (€150 - €130).
De meerwaardebelasting bedraagt €2 (10% van €20).
<br/><br/>
Bron: https://www.bolero.be/nl/lp/meerwaardebelasting
</i></sub>

```mermaid
flowchart TD

    A["Aankoop in 2023<br/>= €100"]

    B["Aankoop in 2024<br/>= €140"]

    C["Gemiddelde aankoopkoers<br/>(GAK) = €120"]

    D["Slotkoers op 31-12-2025<br/>= €130"]

    E{"Is GAK hoger<br/>dan startpunt?"}

    F["Gebruik GAK<br/>als aanschaffingswaarde"]

    G["Gebruik startpunt<br/>als aanschaffingswaarde"]

    H["Verkoopprijs in 2028<br/>= €150"]

    I["Meerwaarde =<br/>€150 - €130 = €20"]

    J["Meerwaardebelasting<br/>10% van €20 = €2"]

    A --> C
    B --> C

    C --> E
    D --> E

    E -->|Ja| F
    E -->|Nee| G

    F --> H
    G --> H

    H --> I
    I --> J
```
