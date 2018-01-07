# Actor/ActorLink/[NAME].bxml
  
  The ``[NAME].bxml`` (Example: ``Enemy_Guardian_A.bxml``) inside the ActorLink folder is primarily used to link several parts of the
  actor together, specify locations of data, and the listings of several tags/flags used for this actor.
  
  ## General Information
  
  - Compression: ``AAMP``
  
  ## Layout
  
  The ``[NAME].bxml`` is split into 2 nodes below 1 root node.
  
  |Name|Index|Description|
  |----|-----|-----------|
  |``param_root``|0 - Root| Root Node.|
  |``LinkTarget``|1|?|
  |``Tags``|2|?|
  
  ## ``LinkTarget`` Properties
  
  The ``LinkTarget`` node contains information regarding the general setup and composition of the actor.
  
  |Name|Type|Description|Default Values|
  |----|----|-----------|--------------|
  |``ActorNameJpn``|*String2*|Name of the actor in japanese.||
  |``Priority``|*String2*|?|``Default``|
  |``AIProgramUser``|*String2*|?||
  |``AIScheduleUser``|*String2*|?||
  |``ASUser``|*String2*|?||
  |``AttentionUser``|*String2*|?||
  |``AwarenessUser``|*String2*|?||
  |``BoneControlUser``|*String2*|?||
  |``ActorCaptureUser``|*String2*|?||
  |``ChemicalUser``|*String2*|?||
  |``DamageParamUser``|*String2*|?||
  |``DropTableUser``|*String2*|?||
  |``ElinkUser``|*String2*|?||
  |``GParamUser``|*String2*|?||
  |``LifeConditionUser``|*String2*|?||
  |``LODUser``|*String2*|?|``EnemyNoCalcSkip``|
  |``ModelUser``|*String2*|?||
  |``PhysicsUser``|*String2*|?||
  |``ProfileUser``|*String2*|?||
  |``RgBlendWeightUser``|*String2*|?||
  |``RgConfigListUser``|*String2*|?||
  |``RecipeUser``|*String2*|?||
  |``ShopDataUser``|*String2*|?||
  |``SlinkUser``|*String2*|?||
  |``UMiiUser``|*String2*|?||
  |``XlinkUser``|*String2*|?||
  |``AnimationInfo``|*String2*|?||
  |``ActorScale``|*Float*|?||
  
  ## ``Tags`` Properties
  
  The ``Tags`` node contains tags/flags for additional information, data and behavior where no node is available in ``LinkTarget``.
  
  |Tag|Description|
  |---|-----------|
  |``RevivalBloodyMoon``|?|
  |``StopTimerShort``|?|
  |``ZukanEnemy``|?|
  |``AllRadarActor``|?|
  |``EffectiveAncientArrow``|?|
  |``AncientGuardTarget``|?|
  |``TeamGuardian``|?|
  
  ***
  
  ## Example
  
  - Example File: ``Enemy_Guardian_A/ActorLink/Enemy_Guardian_A.bxml``

  ```xml
  <param_root children="2">
    <LinkTarget children="28">
        <ActorNameJpn type="string2">ガーディアン（歩行型）</ActorNameJpn>
        <Priority type="string2">Default</Priority>
        <AIProgramUser type="string2">Guardian_A</AIProgramUser>
        <AIScheduleUser type="string2">Dummy</AIScheduleUser>
        <ASUser type="string2">Enemy_Guardian_A</ASUser>
        <AttentionUser type="string2">Guardian_A</AttentionUser>
        <AwarenessUser type="string2">Guardian</AwarenessUser>
        <BoneControlUser type="string2">Dummy</BoneControlUser>
        <ActorCaptureUser type="string2">Dummy</ActorCaptureUser>
        <ChemicalUser type="string2">Dummy</ChemicalUser>
        <DamageParamUser type="string2">Guardian</DamageParamUser>
        <DropTableUser type="string2">Enemy_Guardian_A</DropTableUser>
        <ElinkUser type="string2">Guardian_A</ElinkUser>
        <GParamUser type="string2">Enemy_Guardian_A</GParamUser>
        <LifeConditionUser type="string2">Enemy_Guardian_A</LifeConditionUser>
        <LODUser type="string2">EnemyNoCalcSkip</LODUser>
        <ModelUser type="string2">Enemy_Guardian_A</ModelUser>
        <PhysicsUser type="string2">Enemy_Guardian_A</PhysicsUser>
        <ProfileUser type="string2">Guardian</ProfileUser>
        <RgBlendWeightUser type="string2">Dummy</RgBlendWeightUser>
        <RgConfigListUser type="string2">Dummy</RgConfigListUser>
        <RecipeUser type="string2">Dummy</RecipeUser>
        <ShopDataUser type="string2">Dummy</ShopDataUser>
        <SlinkUser type="string2">Guardian</SlinkUser>
        <UMiiUser type="string2">Dummy</UMiiUser>
        <XlinkUser type="string2">Guardian</XlinkUser>
        <AnimationInfo type="string2">Dummy</AnimationInfo>
        <ActorScale type="float">1</ActorScale>
    </LinkTarget>
    <Tags children="7">
        <node type="string2">RevivalBloodyMoon</node>
        <node type="string2">StopTimerShort</node>
        <node type="string2">ZukanEnemy</node>
        <node type="string2">AllRadarActor</node>
        <node type="string2">EffectiveAncientArrow</node>
        <node type="string2">AncientGuardTarget</node>
        <node type="string2">TeamGuardian</node>
    </Tags>
  </param_root>```
    
