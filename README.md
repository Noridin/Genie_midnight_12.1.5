# Genie – 12.1.5 Community Update

Community-maintained update of the **Genie** bag/bank/guild bank sorter for World of Warcraft 12.1.5 (Interface 120105).

## Changes in this update

- Updated for Interface **120105**
- Replaced removed APIs with the new `C_Item` namespace:
  - `GetItemFamily` → `C_Item.GetItemFamily`
  - `GetItemInfo` → `C_Item.GetItemInfo`
  - `GetItemClassInfo` → `C_Item.GetItemClassInfo`
  - `GetItemSubClassInfo` → `C_Item.GetItemSubClassInfo`
  - `GetItemQualityColor` → `C_Item.GetItemQualityColor`
- Config mode (Shift+Right Click) menu works again on inventory items
- Warband Bank (Account Bank tabs) is now excluded from sorting so Warbound items stay put
- Relies on the standalone **Ace3** addon instead of embedded libraries

## Requirements

- [Ace3](https://www.curseforge.com/wow/addons/ace3)

## Install

1. Delete any old `Genie`, `Genie_UI`, and `Genie_LDB` folders from `Interface/AddOns/`
2. Extract this archive so the three folders land directly in `AddOns/`
3. Type `/reload` in game

## Modules

| Folder       | Purpose                          |
|--------------|----------------------------------|
| `Genie`      | Core sorting engine              |
| `Genie_UI`   | Ranking editor / config window   |
| `Genie_LDB`  | Minimap / LibDataBroker button   |

You can disable `Genie_UI` or `Genie_LDB` in the addon list if you only want the sorter.

## Original project

- CurseForge: https://www.curseforge.com/wow/addons/genie
- Author: adjoeu
