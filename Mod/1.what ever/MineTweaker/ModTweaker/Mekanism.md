## **Handlers Supported**

The following handlers are supported:

- Chemical Crystallizer
- Chemical Dissolution Chamber
- Chemical Infuser
- Chemical Injection Chamber
- Chemical Oxidizer
- Chemical Washer
- Combiner
- Osmium Compressor
- Crusher
- Energized Smelter
- Enrichment Chamber
- Metallurgic Infuser
- Purification Chamber
- Pressurised Reaction Chamber
- Precision Sawmill
- Electrolytic Seperator
- Solar Evaporation
- Solar Neutron Activator

Each of these handlers can have recipes added or removed:

> Parameters marked as red are optional and can be left out

- Chemical Crystallizer

```
//InputGas, OutputStack
mods.mekanism.chemical.Crystallizer.addRecipe(<gas:water>, <minecraft:ice>);

//OutputStack, InputGas
mods.mekanism.chemical.Crystallizer.removeRecipe(<Mekanism:OtherDust:4>, <gas:lithium>);
```

- Chemical Dissolution Chamber

```
//InputStack, OutputGas
mods.mekanism.chemical.Dissolution.addRecipe(<minecraft:ice>, <gas:water>);

//OutputGas, InputStack
mods.mekanism.chemical.Dissolution.removeRecipe(<gas:osmium>, <Mekanism:OreBlock>);
```

- Chemical Infuser

```
//InputGas1, InputGas2, OutputGas
mods.mekanism.chemical.Infuser.addRecipe(<gas:water>, <gas:deuterium>, <gas:steam>);

//OutputGas, InputGas1, InputGas2
mods.mekanism.chemical.Infuser.removeRecipe(<gas:hydrogenchloride>, <gas:hydrogen>, <gas:chlorine>);
```

- Chemical Injection Chamber

```
//InputStack, InputGas, OutputStack
//InputGas only accepts "<gas:sulfuricAcid>", "<gas:water>" or "<gas:hydrogenChloride>"
mods.mekanism.chemical.Injection.addRecipe(<minecraft:hardened_clay:1>, <gas:water>, <minecraft:clay>);

//OutputStack, InputStack, InputGas
mods.mekanism.chemical.Injection.removeRecipe(<Mekanism:Shard:2>, <Mekanism:OreBlock>, <gas:hydrogenchloride>);
```

- Chemical Oxidizer

```
//InputStack, OutputGas
mods.mekanism.chemical.Oxidizer.addRecipe(<Mekanism:Dust:2>, <gas:cleanOsmium>);

//OutputGas, InputStack
mods.mekanism.chemical.Oxidizer.removeRecipe(<gas:brine>, <Mekanism:Salt>);
```

- Chemical Washer

```
//InputGas, OutputGas
mods.mekanism.chemical.Washer.addRecipe(<gas:steam>, <gas:water>);

//OutputGas, InputGas
mods.mekanism.chemical.Washer.removeRecipe(<gas:cleanLead>, <gas:lead>);
```

- Combiner

```
//InputStack, InputGas, OutputStack
mods.mekanism.Combiner.addRecipe(<minecraft:stone> * 4, <gas:liquidStone>, <minecraft:stonebrick>);

//OutputStack, InputStack, InputGas
mods.mekanism.Combiner.removeRecipe(<minecraft:gravel>, <minecraft:flint>, <gas:liquidStone>);
```

- Osmium Compressor

```
//InputStack, InputGas, OutputStack
mods.mekanism.Compressor.addRecipe(<Mekanism:BasicBlock:3>, <gas:liquidOsmium>, <minecraft:bedrock>);

//OutputStack, InputStack, InputGas
mods.mekanism.Compressor.removeRecipe(<Mekanism:Ingot>, <Mekanism:OtherDust:5>, <gas:liquidOsmium>);
```

- Crusher

```
//InputStack, OutputStack
mods.mekanism.Crusher.addRecipe(<minecraft:double_plant:4>, <minecraft:dye:1> * 5);

//OutputStack, InputStack
mods.mekanism.Crusher.removeRecipe(<minecraft:sand>, <minecraft:gravel>);
```

- Energized Smelter

```
//InputStack, OutputStack
mods.mekanism.Smelter.addRecipe(<minecraft:tallgrass:1>, <minecraft:deadbush>);

//InputStack, OutputStack
mods.mekanism.Smelter.removeRecipe(<minecraft:sand>, <minecraft:glass>);
```

- Enrichment Chamber

```
//InputStack, OutputStack
mods.mekanism.Enrichment.addRecipe(<minecraft:coal_block>, <Mekanism:CompressedCarbon> * 9);

//InputStack, OutputStack
mods.mekanism.Enrichment.removeRecipe(<minecraft:mossy_cobblestone>, <minecraft:cobblestone>);
```

- Metallurgic Infuser

```
//InfusionString, InputInfusion, InputStack, OutputStack //InfusionString = CARBON;TIN;DIAMOND;REDSTONE;FUNGI;BIO;OBSIDIAN
mods.mekanism.Infuser.addRecipe("OBSIDIAN", 20, <minecraft:coal_block>, <minecraft:obsidian>);

//OutputStack, InputStack, InfusionString
mods.mekanism.Infuser.removeRecipe(<minecraft:mycelium>);
```

- Purification Chamber

```
//InputStack, InputGas, OutputStack
mods.mekanism.Purification.addRecipe(<minecraft:wool:1>, <gas:hydrogenchloride>, <minecraft:wool>);

//OutputStack, InputStack, InputGas
mods.mekanism.Purification.removeRecipe(<Mekanism:Clump:2>, <Mekanism:Shard:2>, <gas:oxygen>);
```

- Pressurised Reaction Chamber

```
//InputStack, InputFluid, InputGas, OutputStack, OutputGas, InputRF, Time in Ticks
mods.mekanism.Reaction.addRecipe(<Mekanism:Polyethene>, <liquid:ethene>, <gas:oxygen>, <Mekanism:Polyethene> * 8, <gas:oxygen>, 50000, 2000);

//OutputStack, OutputGas, InputStack, InputFluid, InputGas
mods.mekanism.Reaction.removeRecipe(<Mekanism:Substrate>, <gas:ethene>, <Mekanism:BioFuel>, <liquid:water>, <gas:hydrogen>);
```

- Precision Sawmill

```
//InputStack, OutputStack1, OutputStack2, Chance
mods.mekanism.Sawmill.addRecipe(<minecraft:bow>, <minecraft:stick> * 3, <minecraft:string> * 3, 0.5);

//InputStack, OutputStack1, OutputStack2
mods.mekanism.Sawmill.removeRecipe(<minecraft:bed>, <minecraft:planks>, <minecraft:wool>);
```

- Electrolytic Separator

```
//InputFluid, InputRF, OutputGas1, OutputGas2
mods.mekanism.Separator.addRecipe(<liquid:fusionfueldt>, 5000, <gas:deuterium>, <gas:tritium>);

//InputFluid, OutputGas1, OutputGas2
mods.mekanism.Separator.removeRecipe(<liquid:heavywater>, <gas:deuterium>, <gas:oxygen>);
```

- Solar Evaporation

```
//InputFluid, OutputFluid
mods.mekanism.SolarEvaporation.addRecipe(<liquid:lava>, <liquid:fusionfueldt>);

//InputFluid, OutputFluid
mods.mekanism.SolarEvaporation.removeRecipe(<liquid:water>, <liquid:brine>);
```

- Solar Neutron Activator 

```
//InputGas, OutputGas
mods.mekanism.SolarNeutronActivator.addRecipe(<gas:liquidStone>, <gas:liquidOsmium>);

//InputGas, OutputGas
mods.mekanism.SolarNeutronActivator.removeRecipe(<gas:lithium>, <gas:tritium>);
```

## **Commands Supported**

Prints are stored in the minetweaker log in the minecraft directory.

- `/minetweaker mekanism [HANDLER]` - Outputs a list of all Mekansm recipes
- `/minetweaker gases` - Outputs a list of gases