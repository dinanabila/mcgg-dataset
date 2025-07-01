# Magic Chess: Go Go Hero & Card Reference Dataset

This repository contains **reference datasets** for heroes and cards used in Magic Chess: Go Go. These datasets are intended to complement the [Magic Chess: Go Go Matches Dataset](https://github.com/dinanabila/mcgg-matches-dataset) by providing structured information about hero attributes and card effects in order to enabling more meaningful and accurate analysis.

## 📂 Dataset Structure
The dataset consists of **two csv files**:
### 1. `heroes`

A dataset containing static information about all heroes available in the game.

| Column Name | Description |
|-------------|-------------|
| `Hero`      | Name of the hero |
| `Faction`   | Hero's faction (e.g., DoomSworm, Scarlet Shadow) |
| `Role`      | Hero's role/class (e.g., Bruiser, Defender) |
| `Row`       | Recommended position on the board (`Front` or `Back`) |
| `Cost`      | Hero's mana cost in the shop (1 to 5) |

### 2. `cards`

A dataset describing the attributes and effects of various in-game cards.  
Each card is encoded with **binary features**: `1` indicates that the card has that attribute, and `0` means it does not.

| Column Name         | Description |
|---------------------|-------------|
| `Card`              | Name of the card |
| `Color`             | Card rarity or type (e.g., Orange, Purple) |
| `Magic_Boost`       | Boosts magic damage |
| `Physical_Boost`    | Boosts physical damage |
| `ATKSpeed_Boost`    | Increases attack speed |
| `Defense_Boost`     | Increases defense or durability |
| `Synergy`           | Enhances or interacts with a synergy |
| `Magic_Equipment`   | Provides magic-type equipment |
| `Physical_Equipment`| Provides physical-type equipment |
| `ATKSpeed_Equipment`| Provides attack speed equipment |
| `Defense_Equipment` | Provides defensive equipment |
| `Hero_Recruitment`  | Summons a new hero |
| `Capacity+`         | Increases max team capacity |
| `Economy`           | Boosts economy or gold gain |
| `Commander_EXP`     | Grants Commander experience |
| `Commander_Life`    | Restores Commander HP |
| `Synergy_Effect`    | Modifies synergy effects or adds synergy bonuses |

## 🎯 Purpose

These reference datasets are designed to **support match-level analysis** in the [Magic Chess: Go Go Matches Dataset](https://github.com/dinanabila/mcgg-matches-dataset). They provide additional context such as:

- Hero characteristics for synergy or frontline/backline composition analysis  
- Card effects for evaluating card impact on win rate or synergy boosts  

By linking match data with this reference information, we can uncover deeper patterns and more accurate insights.

## 🧠 Use Cases

- Enhance feature engineering for match analysis
- Map hero usage to roles/factions for synergy analysis
- Analyze the strategic impact of specific card attributes
- Cluster or group cards/heroes by characteristics (e.g., all economy-boosting cards)
