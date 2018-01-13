# DungeonXYZ.bdgnenv

## General Information

- Compression: ``AAMP``

## Layout

The ``DungeonXYZ.bdgnenv`` is split into 1 node below 1 root node.

|Name|Index|Description|
|----|-----|-----------|
|``param_root``|0 - Root| Root Node.|
|``DungeonEnv``|1|?|

## ``DungeonEnv`` Properties

|Name|Type|Description|Default Values|
|----|----|-----------|--------------|
|``LightLongitude``|*Float*|?| Variable.|
|``DungeonSize``|*String*|Identifier for the size of the Dungeon.|``S``, ``M``, ``L``|
|``DungeonType``|*String*|?|``Gimmick``|#
|Unknown ``Hash=4097207359``|*Integer*|?||
|Unknown ``Hash=1214923583``|*Integer*|?||
|Unknown ``Hash=3770696383``|*Boolean*|?||
|Unknown ``Hash=778701914``|*Boolean|?||
|Unknown ``Hash=832345865``|*Boolean*|?||
|Unknown ``Hash=2091617280``|*Boolean*|?||
|``ChemicalType``|*Integer*|?|``1``|

---

## Example

- Example File: ``Dungeon000/Map/DungeonData/CDungeon/Dungeon000.bdgnenv``

```xml
<param_root children="1">
  <DungeonEnv children="10">
    <LightLongitude type="float">300</LightLongitude>
    <DungeonSize type="string">S</DungeonSize>
    <DungeonType type="string">Gimmick</DungeonType>
    <node type="int" hash="4097207359">1</node>
    <node type="int" hash="1214923583">2</node>
    <node type="bool" hash="3770696383">true</node>
    <node type="bool" hash="778701914">false</node>
    <node type="bool" hash="832345865">false</node>
    <node type="bool" hash="2091617280">false</node>
    <ChemicalType type="int">1</ChemicalType>
  </DungeonEnv>
</param_root>
