# Modifiers
## Modifier Files
Modifiers are the core of the Dimension Delvers upgrade system.
### Format
* `modifiers` : A list of modifier effects that will be applied to the entity by this modifier.
### Usage
You select one or more from the modifier effects described below and add it in the `modifiers` list.

### Example

```json
{
  "modifiers": [
    {
      "type": "dimensiondelvers:attribute_modifier",
      "id": "minecraft:flat_attack_damage",
      "attribute": "minecraft:attack_damage",
      "min_roll": 1,
      "max_roll": 3,
      "operation": "add_value"
    }
  ]
}
```
### Note on rolls
A `roll` is used to calculate the correct value of a modifier effect. This roll is a number between 0 and 1. It uses the `roll` value determined by the modifierInstane owner of the modifier.

The final calculation is usually something like: `min_roll + ((max_roll - min_roll) * roll)`

## AttributeModifierEffect
### Format
* `type`: `"dimensiondelvers:attribute"`
* `id`: The id is used to uniquely identify this attribute modifier efect in the list of modifier effects for this modifier. This is necessary to identify the correct attributes to remove when the item is removed.
* `attribute`: The attribute adjusted by this effect.
* `min_roll`: The minimum value that can be rolled for this effect. 
* `max_roll`: The maximum value that can be rolled for this effect.
* `operation`: The operation to perform on the attribute. Can be `add_value`, `add_multiplied_base`, `add_multiplied_total`. See vanilla AttributeModifier for more information.
### Usage
Each effect will add a random value between `min_roll` and `max_roll` to the `attribute` of the entity. The `operation` will determine how the value is added.
### Example
```json
{
  "type": "dimensiondelvers:attribute_modifier",
  "id": "minecraft:flat_attack_damage",
  "attribute": "minecraft:attack_damage",
  "min_roll": 1,
  "max_roll": 3,
  "operation": "add_value"
}
```