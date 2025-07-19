# Lakas ng Lahi - Game Design Document

---

## Overview
A hybrid RTS/action-adventure game inspired by Battle Realms and Ronin Trail, set in a semi-historical, semi-mythological Philippines. Players choose a clan, train unique units, and master both strategic and souls-like combat.

---

## Table of Contents
- [Clans & Philosophy](#clans--philosophy)
- [Unit Training Trees](#unit-training-trees)
- [Tech & Upgrade Trees](#tech--upgrade-trees)
- [Unit Stats & Skills](#unit-stats--skills)
- [Mermaid Diagrams](#mermaid-diagrams)
- [Lore Blurbs](#lore-blurbs)

---

## Clans & Philosophy

### Tagalog
- **Philosophy:** Honor, unity, and resilience. Masters of the kampilan and shield wall tactics.
- **Signature Hero:** Rajah Sulayman

### Visayan
- **Philosophy:** Seafaring, raiding, and adaptability. Naval prowess and swift skirmishers.
- **Signature Hero:** Datu Lapu-Lapu

### Igorot
- **Philosophy:** Guerrilla warfare, nature attunement, and spiritual rituals. Masters of ambush and terrain.
- **Signature Hero:** Apo Anno

### T'boli
- **Philosophy:** Mysticism, dreams, and spiritual guardianship. Unique support and shamanic units.
- **Signature Hero:** Lemlunay

### Maguindanao
- **Philosophy:** Martial discipline, archery, and kris mastery. Balanced offense and defense.
- **Signature Hero:** Sultan Kudarat

---

## Unit Training Trees

### Tagalog Clan
```mermaid
flowchart TD
    T0[Villager] --> T1[Kampilan Trainee]
    T1 --> T2[Kampilan Warrior]
    T2 --> T3[Armored Swordsman]
    T1 --> T4[Shieldbearer]
    T0 --> T5[Spearman]
    T5 --> T6[Elite Spearman]
```

### Visayan Clan
```mermaid
flowchart TD
    V0[Villager] --> V1[Raider Trainee]
    V1 --> V2[Raider]
    V2 --> V3[Naval Raider]
    V1 --> V4[Fisherman]
    V0 --> V5[Scout]
    V5 --> V6[Skirmisher]
```

### Igorot Clan
```mermaid
flowchart TD
    I0[Villager] --> I1[Hunter Trainee]
    I1 --> I2[Hunter]
    I2 --> I3[Headhunter]
    I1 --> I4[Ritualist]
    I0 --> I5[Slinger]
    I5 --> I6[Ambusher]
```

### T'boli Clan
```mermaid
flowchart TD
    B0[Villager] --> B1[Spirit Novice]
    B1 --> B2[Babaylan]
    B2 --> B3[Spirit Shaman]
    B1 --> B4[Herbalist]
    B0 --> B5[Mystic Guard]
    B5 --> B6[Dreamweaver]
```

### Maguindanao Clan
```mermaid
flowchart TD
    M0[Villager] --> M1[Kris Trainee]
    M1 --> M2[Kris Fighter]
    M2 --> M3[Elite Kris Warrior]
    M1 --> M4[Shieldbearer]
    M0 --> M5[Archer]
    M5 --> M6[Marksman]
```

---

## Tech & Upgrade Trees

```mermaid
flowchart TD
    Start[Basic Tech] --> Tactics[Clan Tactics]
    Tactics --> Weapons[Weapon Upgrades]
    Tactics --> Armor[Armor Upgrades]
    Weapons --> Elite[Elite Training]
    Armor --> Fortify[Fortifications]
    Elite --> Hero[Hero Unlock]
```

---

## Unit Stats & Skills

| Clan        | Unit                | HP  | ATK | DEF | Skills                |
|-------------|---------------------|-----|-----|-----|-----------------------|
| Tagalog     | Kampilan Warrior    | 120 | 30  | 10  | Kampilan Charge       |
| Tagalog     | Armored Swordsman   | 160 | 38  | 18  | Shield Wall           |
| Visayan     | Raider              | 110 | 28  | 8   | Sea Raid              |
| Visayan     | Naval Raider        | 130 | 32  | 12  | Boarding Party        |
| Igorot      | Hunter              | 100 | 26  | 8   | Forest Ambush         |
| Igorot      | Headhunter          | 140 | 36  | 14  | Trophy Hunt           |
| T'boli      | Babaylan            | 90  | 18  | 6   | Spirit Heal           |
| T'boli      | Spirit Shaman       | 110 | 22  | 10  | Dreamweave            |
| Maguindanao | Kris Fighter        | 115 | 29  | 9   | Kris Flurry           |
| Maguindanao | Marksman            | 105 | 34  | 7   | Eagle Eye             |

---

## Mermaid Diagrams

### Clan System Overview
```mermaid
graph TD
  Player --> ClanSelect[Select Clan]
  ClanSelect --> Tagalog
  ClanSelect --> Visayan
  ClanSelect --> Igorot
  ClanSelect --> Tboli
  ClanSelect --> Maguindanao
```

### Skill Activation Flow
```mermaid
graph TD
  Player/AI -->|Trigger| SkillSystem
  SkillSystem -->|Check Cooldown| SkillReady{Ready?}
  SkillReady -- No --> UI[Show Cooldown]
  SkillReady -- Yes --> ApplyEffect[Apply Effect]
  ApplyEffect --> Animation[Play Animation]
  ApplyEffect --> StatChange[Modify Stats]
  ApplyEffect --> VFX[Show VFX]
```

### Upgrade Flow
```mermaid
graph TD
  Villager --> BasicUnit
  BasicUnit --> AdvancedUnit
  AdvancedUnit --> EliteUnit
  BasicUnit --> SupportUnit
  BasicUnit --> RangedUnit
```

---

## Lore Blurbs

- **Tagalog:** The Tagalog warriors, led by Rajah Sulayman, are renowned for their discipline and shield tactics, defending their homeland with honor.
- **Visayan:** The Visayan raiders, under Datu Lapu-Lapu, rule the seas and strike swiftly, their courage legendary among the islands.
- **Igorot:** The Igorot clans, guided by Apo Anno, blend into the mountains, striking unseen and vanishing like spirits.
- **T'boli:** The T'boli, with Lemlunay as their spiritual guide, weave dreams and reality, healing and protecting their kin.
- **Maguindanao:** The Maguindanao, led by Sultan Kudarat, are masters of the kris and bow, balancing martial might with wisdom.

---

*For more details, see [lore-bible.md](./lore-bible.md), [moodboard.md](./moodboard.md), and [web3-integration.md](./web3-integration.md).* 