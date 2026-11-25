# Berekening meerwaardebelasting, Bolero example 5.2

<sub><i>
Voorbeeld 2: verkoop van aandelen die je in verschillende keren kocht, waarbij je aandelen kocht vóór 2026 met een aankoopkoers hoger dan de slotkoers op 31-12-2025.
De slotkoers op 31-12-2025 bedraagt €100 per aandeel. De verkoopkoers in 2027 bedraagt €130 per aandeel.
In 2019 koop je 50 aandelen aan €120. In 2024 koop je 40 aandelen aan €110.
Je bezit daardoor 90 aandelen met een gemiddelde aankoopprijs (GAK) van €115,56.
Omdat deze aankoopprijzen hoger liggen dan de slotkoers van €100 op 31-12-2025, mag de gemiddelde aankoopprijs als startbasis worden gebruikt.
In 2026 koop je vervolgens 30 aandelen aan €95 en nog eens 20 aandelen aan €105.
In 2027 verkoop je 126 aandelen aan €130 per aandeel.
Volgens de fiscale FIFO-regel (First In First Out) worden eerst de oudste aandelen verkocht: 2019 → 2024 → 2026 (eerste aankoop) → 2026 (tweede aankoop).
De verkoopopbrengst bedraagt €16.380 (126 × €130).
De fiscale kostprijs bedraagt €13.880:
90 aandelen × €115,56 ≈ €10.400,
30 aandelen × €95 = €2.850,
6 aandelen × €105 = €630.
De belastbare meerwaarde bedraagt €2.500 (€16.380 - €13.880).
De verschuldigde meerwaardebelasting bedraagt €250 (10% van €2.500).

<br/><br/>
Bron: https://www.bolero.be/nl/lp/meerwaardebelasting
</i></sub>

```mermaid
flowchart TD

    A["2019<br/>Koop 50 aandelen<br/>à €120"]

    B["2024<br/>Koop 40 aandelen<br/>à €110"]

    C["90 aandelen<br/>GAK = €115,56"]

    D["Slotkoers 31-12-2025<br/>= €100"]

    E{"GAK hoger dan<br/>startpunt?"}

    F["Gebruik GAK<br/>€115,56"]

    G["2026<br/>Koop 30 aandelen<br/>à €95"]

    H["2026<br/>Koop 20 aandelen<br/>à €105"]

    I["2027<br/>Verkoop 126 aandelen<br/>à €130"]

    J["FIFO-verwerking"]

    K["90 aandelen<br/>aan €115,56<br/>= €10.400"]

    L["30 aandelen<br/>aan €95<br/>= €2.850"]

    M["6 aandelen<br/>aan €105<br/>= €630"]

    N["Totale kostprijs<br/>= €13.880"]

    O["Verkoopopbrengst<br/>= €16.380"]

    P["Belastbare meerwaarde<br/>= €2.500"]

    Q["Meerwaardebelasting<br/>10% = €250"]

    A --> C
    B --> C

    C --> E
    D --> E

    E -->|Ja| F

    F --> J
    G --> J
