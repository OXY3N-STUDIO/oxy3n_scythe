# Make the scythe a weapon for QBCore

## Installation
- Put the ``oxy3n_scythe`` into your ``resources`` folder.

## Drop first code in ``qb-core/shared/items.lua``
```lua
	['weapon_scythe'] = {['name'] = 'weapon_scythe', ['label'] = 'Scythe', ['weight'] = 1000, ['type'] = 'weapon', ['ammotype'] = nil, ['image'] = 'scythe.png', ['unique'] = true, ['useable'] = false, ['description'] = ''},
```

## Drop the next code in ``qb-core/shared/weapons.lua``

```lua
	[`weapon_scythe`] = {['name'] = 'weapon_scythe', ['label'] = 'Scythe', ['ammotype'] = nil, ['damagereason'] = 'Scythed / Stabbed / Eviscerated'},
```

## Drop the next code in ``qb-weapons/config.lua``

```lua
    ['weapon_scythe'] 				 = 0.15,
```

Drop the scythe.png in ``qb-inventory/html/images`` for inventory image