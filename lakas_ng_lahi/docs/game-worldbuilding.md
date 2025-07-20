# Game Worldbuilding

---

## Major Places
- **Maynila:** Capital city, Tagalog stronghold, center of trade and politics.
- **Balangay Isles:** Visayan seafaring villages, naval bases.
- **Cordillera Highlands:** Igorot mountain settlements, terraced fields.
- **Lake Sebu:** T'boli spiritual center, dreamweaver villages.
- **Cotabato Plains:** Maguindanao fortresses, lush farmlands.
- **Northern Wilds:** Untamed forests, bandit camps, rare resources.
- **Southern Delta:** Swamps, hidden shrines, amphibious routes.
- **Central Plateau:** Trade crossroads, neutral towns, contested territory.
- **Eastern Reaches:** Coastal villages, fishing grounds, pirate coves.

---

## Inhabitants & Cultures
- **Tagalog:** Urban, disciplined, honor-bound.
- **Visayan:** Seafaring, adaptable, bold.
- **Igorot:** Nature-attuned, spiritual, guerrilla fighters.
- **T'boli:** Mystical, artistic, dreamweavers.
- **Maguindanao:** Martial, wise, balanced.

---

## Bug Report
| ID | Description | Location | Status |
|----|-------------|----------|--------|
| 1  | Example bug | Maynila   | Open   |

---

## Combined World Map (RTS + Velarde Style)
This map combines the detailed, game-like RTS layout with the historical, archipelagic flow inspired by the [Velarde Map of 1734](https://en.wikipedia.org/wiki/Velarde_map#/media/File:Carta_Hydrographica_y_Chorographica_de_las_Yslas_Filipinas_Dedicada_al_Rey_Nuestro_Se%C3%B1or_por_el_Mariscal_d._Campo_D._Fernando_Valdes_Tamon_Cavall%C2%BA_del_Orden_de_Santiago_de_Govor._Y_Capn.jpg). Regions are grouped by geography and culture, with strategic points and routes for gameplay, while also reflecting the north-to-south island chain of the Philippines.

```mermaid
flowchart TD
  %% Luzon/North
  subgraph "Luzon (North)"
    LU1["Cordillera Highlands\n(Igorot)"]
    LU2["Maynila\n(Tagalog Capital)"]
    LU3["Cagayan Valley"]
    LU4["Ilocos Coast"]
    NW1["Northern Wilds"]
    CH1["Igorot Village"]
    CH2["Terraced Fields"]
    M1["Palace"]
    M2["Market"]
    M3["Harbor"]
  end

  %% Central Islands
  subgraph "Central Islands"
    CI1["Balangay Isles\n(Visayan)"]
    CI2["Panay"]
    CI3["Cebu"]
    CI4["Bohol"]
    CI5["Samar"]
    CI6["Leyte"]
    BI1["Naval Base"]
    BI2["Fishing Village"]
  end

  %% Mindanao/South
  subgraph "Mindanao (South)"
    MI1["Cotabato Plains\n(Maguindanao)"]
    MI2["Lake Sebu\n(T'boli)"]
    MI3["Zamboanga"]
    MI4["Davao"]
    MI5["Sulu Archipelago"]
    CP1["Fortress"]
    CP2["Rice Fields"]
    LS1["Dreamweaver Village"]
    LS2["Sacred Lake"]
  end

  %% Other Regions
  subgraph "Frontier & Seas"
    FS1["Northern Wilds"]
    FS2["Eastern Reaches"]
    FS3["Southern Delta"]
    FS4["Western Shoals"]
    SD1["Swamp Shrine"]
    SD2["Hidden Path"]
    ER1["Fishing Grounds"]
    ER2["Pirate Cove"]
    CTP1["Trade Town"]
    CTP2["Crossroads"]
  end

  %% Main archipelagic flow (Velarde style)
  FS1 -- "Mountain Pass" --> LU1
  LU1 -- "River Road" --> LU2
  LU2 -- "Trade Route" --> LU3
  LU3 -- "Coastal Path" --> LU4
  LU2 -- "Sea Crossing" --> CI1
  LU4 -- "Merchant Fleet" --> CI2
  CI1 -- "Island Ferry" --> CI2
  CI2 -- "Bridge" --> CI3
  CI3 -- "Raft" --> CI4
  CI4 -- "Fishing Route" --> CI5
  CI5 -- "Pilgrim Trail" --> CI6
  CI6 -- "Southern Passage" --> MI1
  MI1 -- "Jungle Road" --> MI2
  MI2 -- "River Delta" --> MI3
  MI3 -- "Coastal Road" --> MI4
  MI4 -- "Archipelago Route" --> MI5
  MI5 -- "Open Sea" --> FS3
  FS3 -- "Hidden Channel" --> FS2
  FS2 -- "Stormy Waters" --> FS4
  FS4 -- "Pirate Lane" --> LU2

  %% RTS-style strategic connections
  NW1 -- "Forest Path" --> CH1
  CH1 -- "Mountain Road" --> M1
  M1 -- "River Route" --> BI1
  BI1 -- "Sea Lane" --> LS1
  LS1 -- "Pilgrimage Trail" --> CP1
  CP1 -- "Farming Road" --> SD1
  SD1 -- "Delta Crossing" --> CTP1
  CTP1 -- "Trade Route" --> ER1
  ER1 -- "Coastal Path" --> M3
  M3 -- "Harbor Ferry" --> BI2
  CTP2 -- "Neutral Zone" --> M2
  CH2 -- "Terrace Walk" --> CTP2
  NW1 -- "Hidden Track" --> SD2
  SD2 -- "Secret Tunnel" --> CP2
  LS2 -- "Lake Passage" --> ER2

  %% Key cities and capitals
  LU2:::capital
  CI1:::capital
  MI1:::capital
  MI2:::spiritual

  classDef capital fill:#f9e79f,stroke:#b7950b,stroke-width:2px;
  classDef spiritual fill:#aed6f1,stroke:#2874a6,stroke-width:2px;
```

---

*This combined map visually merges the strategic, game-like layout with the historical archipelagic structure, suitable for both gameplay and lore/worldbuilding.* 