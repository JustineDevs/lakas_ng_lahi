# Lakas ng Lahi - Architecture

---

## Overview
Lakas ng Lahi is built as a modular hybrid RTS/action-adventure game using Unreal Engine 5, with optional Web3 integration for NFTs and player-owned assets. The architecture is designed for scalability, maintainability, and cultural authenticity.

---

## System Architecture

```mermaid
graph TD
  Player -->|Input| GameClient
  GameClient -->|Blueprints/C++| GameLogic
  GameLogic -->|Data| ClanSystem
  GameLogic -->|Data| UnitSystem
  GameLogic -->|Data| CombatSystem
  GameLogic -->|Saves| SaveSystem
  GameClient -->|UI| HUD
  GameClient -->|Network| Web3Module
  Web3Module -->|API| Blockchain
```

- **GameClient:** Handles player input, UI, and rendering.
- **GameLogic:** Core gameplay logic (RTS, action, AI, etc.) in C++/Blueprints.
- **ClanSystem:** Manages clans, units, upgrades, and lore.
- **UnitSystem:** Handles unit stats, skills, and training trees.
- **CombatSystem:** Souls-like combat, skills, and effects.
- **SaveSystem:** Local and cloud saves.
- **Web3Module:** Optional; manages NFT, wallet, and blockchain interactions.
- **Blockchain:** Polygon smart contracts for NFTs, land, and marketplace.

---

## Clan & Unit System Flow

```mermaid
flowchart TD
  SelectClan[Select Clan] --> SpawnBase[Spawn Base]
  SpawnBase --> TrainVillager[Train Villager]
  TrainVillager --> UnitTree[Unit Training Tree]
  UnitTree --> Upgrade[Upgrade/Tech Tree]
  Upgrade --> HeroUnlock[Hero Unlock]
```

---

## Skill Activation Flow

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

---

## Web3 Integration
- **Chain:** Polygon (Matic)
- **NFTs:** ERC-721/1155 for cosmetics, land, and anting-anting
- **Wallets:** MetaMask, WalletConnect
- **Marketplace:** Decentralized, in-game UI

### Web3 User Flow
```mermaid
graph TD
  Player --> Wallet[Connect Wallet]
  Wallet --> NFTMint[Mint NFT]
  NFTMint --> Marketplace[Trade on Marketplace]
  Marketplace --> Game[Use in Game]
```

---

## Modular Design Principles
- **Blueprints & C++:** Core systems are modular and extensible.
- **Clan/Unit Data:** Easily add new clans, units, or skills via data tables.
- **Web3 Optional:** Game is fully playable without blockchain features.
- **Cultural Authenticity:** All content reviewed for accuracy and respect.

---

*For more details, see [game-design.md](./game-design.md), [web3-integration.md](./web3-integration.md), and [lore-bible.md](./lore-bible.md).* 