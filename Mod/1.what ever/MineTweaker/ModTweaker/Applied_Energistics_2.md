## **Handlers Supported**

The following handlers are supported:

- Grinder
- Inscriber

Each of these handlers can have recipes added or removed:

> Parameters marked as red are optional and can be left out

- Grinder

```
//InputStack, OutputStack1, Turns, OutputStack2, OutputStackChance2, OutputStack3, OutputStackChance3
mods.appeng.Grinder.addRecipe(<minecraft:sandstone>, <minecraft:sand> * 2, 4, <minecraft:sand>, 0.8, <minecraft:sand>, 0.6);

//OutputStack
mods.appeng.Grinder.removeRecipe(<minecraft:flint>);
```

- Inscriber

```
//InputArray, plateA, plateB, OutputStack, TypeString 
//TypeStrings available are "Inscribe" and "Press"
mods.appeng.Inscriber.addRecipe([<minecraft:gold_block>], <appliedenergistics2:item.ItemMultiMaterial:15>, null, <appliedenergistics2:item.ItemMultiMaterial:18> * 9, "Press");
mods.appeng.Inscriber.addRecipe([<minecraft:iron_ingot>], <minecraft:redstone>, <minecraft:cobblestone>, <minecraft:piston>, "Inscribe");

//OutputStack
mods.appeng.Inscriber.removeRecipe(<appliedenergistics2:item.ItemMultiMaterial:15>);
```