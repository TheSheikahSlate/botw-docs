# Map/MainField/X-Y/X-Y_Dynamic.smubin

## General Information

- Compression: ``BYML``
- Yaz0-Encoded: ``Yes``
## Layout

X-Y_Dynamic.smubin files have a root node Objs with multiple dictionaries (arrays / hash tables) describing map unit objects (i.e. trees, items, mountains, etc.).

## `Objs` Properties

Not all properties are available for all objects

Name | Type | Description | Default Values
---|---|---|---
HashId | Unsigned Int | Unique Id for map unit instance | 
UnitConfigName | String | Name of the object | 
Rotate | Float or List | A list value represents rotation on x, y, z. Float ? | 
Translate | Float or List | A list value represents translation on x, y, z. Float ? |
Scale | Float or List | A list value represents scaling on x, y, z. Float is equal scaling on x, y, z |
SRTHash | Unsigned Int | ? Possibly Scale-Rotate-Translate hash? |
!Parameters | Dictionary | Properties to assign to this map unit instance |

!Parameters values are dependant on the unit type

---

## Example

-Example File: `Map/MainField/A-1/A-1_Dynamic.mubin`

```yaml
- Objs:
  - '!Parameters': {AngleY: 0.0, CutRate: 0.0, DropTable: Normal, SharpWeaponJudgeType: 0}
    HashId: 11472148
    Rotate: 3.006002426147461
    SRTHash: 4159291519
    Translate: [-4046.613525390625, 300.58489990234375, -3327.34228515625]
    UnitConfigName: Obj_TreeConiferous_A_Snow_01
  - '!Parameters': {DropTable: Normal, InitMotionStatus: 0, IsEnemyLiftable: true,
      IsPlayerPut: false, SharpWeaponJudgeType: 0}
    HashId: 17175408
    Rotate: [-1.8166382312774658, -0.30297359824180603, 3.120814561843872]
    SRTHash: 3065466971
    Translate: [-4080.424560546875, 483.92034912109375, -3733.233154296875]
    UnitConfigName: Item_Plant_O
  - '!Parameters': {DropTable: Normal, InitMotionStatus: 0, IsEnemyLiftable: true,
      IsPlayerPut: false, SharpWeaponJudgeType: 0}
    HashId: 35632469
    Rotate: [-1.5354002714157104, -0.4576415717601776, 2.599731206893921]
    SRTHash: ''
    Translate: [-3990.58203125, 241.47265625, -3855.3984375]
    UnitConfigName: Item_Mushroom_D
  - HashId: 36278001
    Rotate: [-0.12477642297744751, 1.2389897108078003, -0.7003511190414429]
    SRTHash: 2146414221
    Scale: 1.0019530057907104
    Translate: [-4094.06640625, 451.7535400390625, -3494.10546875]
    UnitConfigName: Obj_Plant_CypressLow_B_01
  - HashId: 40448728
    Rotate: -3.1415927410125732
    SRTHash: 866874463
    Translate: [-4399.00634765625, 329.0694274902344, -3780.210693359375]
    UnitConfigName: FldObj_KorokStone_A_01
  - '!Parameters': {DropTable: Normal, SharpWeaponJudgeType: 0}
    HashId: 70299346
    Rotate: [2.920030117034912, -0.9325111508369446, 2.9017539024353027]
    SRTHash: 3353710978
    Translate: [-4372.3408203125, 492.61175537109375, -3585.74755859375]
    UnitConfigName: Obj_Mineral_A_01
```
