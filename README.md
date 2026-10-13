# KitsuneMoreSloots

More slots where it counts, for 7 Days to Die V3.0.x through V3.2. Verified against
V3.1 (Henpocalypse) and V3.2: all patched windows (`windowForgeInput`,
`windowCraftingQueue`, `windowOutput`) are unchanged.

- **Forge input:** 2 slots to 3 (an engine limit: the game hardcodes 3 raw input slots; vanilla only displays 2 of them)
- **Crafting / scrapping queue:** 4 slots to 10 (2 rows of 5)
- **Workstation output:** 6 slots to 9 (workbench, forge, campfire, chemistry station, cement mixer)
- **Junk drone storage:** 16 slots to 32 (8 wide, so each cargo mod still adds one full row of 8)

Pure XML modlet (XPath patches only), no DLLs.

## Install

Drop the `KitsuneMoreSloots` folder into your `Mods` folder. Needed on **both server and client**: the slot layouts are client-side UI, so players without the mod will not see the extra slots.

## Notes

- Changing workstation slot counts can clear items sitting inside already-placed workstations on first load. Empty your forges before updating a live save.
- The drone storage size is server-side data (`loot.xml`), so it only takes effect when the server runs the mod. Drones grow to the new size the next time they load; removing the mod later shrinks them back to 16 slots, and anything in the extra slots is lost, so empty your drone first.
- Part of the Kitsune QoL family: [KitsuneBackpack](https://github.com/AdaInTheLab/KitsuneBackpack), [KitsuneStorage](https://github.com/AdaInTheLab/KitsuneStorage).
