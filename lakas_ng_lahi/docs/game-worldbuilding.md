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

## World Map (Mermaid)
```mermaid
flowchart TD
  subgraph "Northern Wilds"
    NW1["Bandit Camp"]
    NW2["Ancient Forest"]
  end
  subgraph "Cordillera Highlands"
    CH1["Igorot Village"]
    CH2["Terraced Fields"]
  end
  subgraph "Maynila"
    M1["Palace"]
    M2["Market"]
    M3["Harbor"]
  end
  subgraph "Balangay Isles"
    BI1["Naval Base"]
    BI2["Fishing Village"]
  end
  subgraph "Lake Sebu"
    LS1["Dreamweaver Village"]
    LS2["Sacred Lake"]
  end
  subgraph "Cotabato Plains"
    CP1["Fortress"]
    CP2["Rice Fields"]
  end
  subgraph "Southern Delta"
    SD1["Swamp Shrine"]
    SD2["Hidden Path"]
  end
  subgraph "Central Plateau"
    CTP1["Trade Town"]
    CTP2["Crossroads"]
  end
  subgraph "Eastern Reaches"
    ER1["Fishing Grounds"]
    ER2["Pirate Cove"]
  end

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
  NW2 -- "Hidden Track" --> SD2
  SD2 -- "Secret Tunnel" --> CP2
  LS2 -- "Lake Passage" --> ER2
```

---

*Expand with new places, cultures, and bug reports as the world grows.* 