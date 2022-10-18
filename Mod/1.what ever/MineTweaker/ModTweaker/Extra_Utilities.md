## **Handlers Supported**

The following handlers are supported:

- QED

Each of these handlers can have recipes added or removed:

> Parameters marked as red are optional and can be left out

- QED Recipes

```
//OutputStack, InputArray
mods.extraUtils.QED.addShapedRecipe(<ExtraUtilities:decorativeBlock1:1> * 8, 
    [[null, <minecraft:obsidian>, null],
    [<minecraft:obsidian>, <minecraft:ender_pearl>, <minecraft:obsidian>], 
    [null, <minecraft:obsidian>, null]]); 

//OutputStack
mods.extraUtils.QED.removeRecipe(<ExtraUtilities:extractor_base_remote>);
```