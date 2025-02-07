# /execute Command Guide

The `/execute` command can be used to apply an action to specific entities, based on conditions such as the items in their inventory or main hand.

---

### Command 1: Give a Specific Item to Anyone with a Specific Item in Their Inventory

This command checks if an entity has a specific item in their inventory and gives them another item if true.

#### Syntax:
> execute as @e[nbt={Inventory:[{id:"minecraft:$item$"}]}] run give @s minecraft:$item$

#### Example:
This example gives anyone who has a dirt block in their inventory a diamond:
> execute as @e[nbt={Inventory:[{id:"minecraft:dirt"}]}] run give @s minecraft:diamond
> 
- **$item$**: Replace with the item you want to check for in the inventory (e.g., `dirt`, `stone`, etc.).
- **minecraft:diamond**: The item to be given when the condition is met.

---

### Command 2: Give a Specific Item to Anyone Holding a Specific Item in Their Main Hand

This command checks if an entity has a specific item in their main hand and gives them another item if true.

#### Syntax:
> execute as @e[nbt={SelectedItem:{id:"minecraft:$item$"}}] run give @s minecraft:$item$

#### Example:
This example gives anyone who has a dirt block in their hand a diamond:
> execute as @e[nbt={SelectedItem:{id:"minecraft:dirt"}}] run give @s minecraft:diamond

- **$item$**: Replace with the item you want to check for in the main hand (e.g., `dirt`, `stone`, etc.).
- **minecraft:diamond**: The item to be given when the condition is met.

---

### Additional Notes:
- These commands will apply to all entities that meet the specified conditions (`@e` targets all entities).
- Replace `$item$` with the item of your choice, and replace the item after `minecraft:` with whatever you wish to give (e.g., `minecraft:diamond`, `minecraft:iron_sword`, etc.).
