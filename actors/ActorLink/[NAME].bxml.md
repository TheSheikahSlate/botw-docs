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
  |``AIProgramUser``|*String2*|Specifies which AIProgram/.baiprog file is used for the actor.||
  |``AIScheduleUser``|*String2*|Specifies which AISchedule/.baischedule file is used for the actor.|``Dummy``|
  |``ASUser``|*String2*|Specifies which ASList/.baslist file is used for the actor.||
  |``AttentionUser``|*String2*|Specifies which AttClientList/.batcllist file is used for the actor.||
  |``AwarenessUser``|*String2*|Specifies which Awareness/.bawareness file is used for the actor.||
  |``BoneControlUser``|*String2*|Specifies which BoneControl/.bbonectrl file is used for the actor.||
  |``ActorCaptureUser``|*String2*|?|``Dummy``|
  |``ChemicalUser``|*String2*|Specifies which Chemical/.bchemical file is used for the actor.||
  |``DamageParamUser``|*String2*|Specifies which DamageParam/.bdmgparam file is used for the actor.||
  |``DropTableUser``|*String2*|Specifies which DropTable/.bdrop file is used for the actor.||
  |``ElinkUser``|*String2*|?||
  |``GParamUser``|*String2*|Specifies which GeneralParamList/.bgparamlist file is used for the actor. Parameters for the actor.||
  |``LifeConditionUser``|*String2*|Specifies which LifeCondition/.blifecondition file is used for the actor. Describes when the actor gets deleted or not.||
  |``LODUser``|*String2*|Specifies which LOD/.blod file is used for the actor.|``EnemyNoCalcSkip``|
  |``ModelUser``|*String2*|Specifies which ModelList/.bmodellist file is used for the actor. The model the actor uses.|``None``|
  |``PhysicsUser``|*String2*|Specifies which Physics/.bphysics file is used for the actor.||
  |``ProfileUser``|*String2*|The type of actor.|``WeaponBow``, ``NPC``, ``Enemy``, ``Bullet``|
  |``RgBlendWeightUser``|*String2*|Specifies which RagdollBlendWeight/.brgbw file is used for the actor.||
  |``RgConfigListUser``|*String2*|Specifies which RagdollConfigList/.brgconfiglist file is used for the actor.||
  |``RecipeUser``|*String2*|Specifies which Recipe/.brecipe file is used for the actor.||
  |``ShopDataUser``|*String2*|Specifies which ShopData/.bshop file is used for the actor.||
  |``SlinkUser``|*String2*|Sound link user.||
  |``UMiiUser``|*String2*|Specifies which UMii/.bumii file is used for the actor. Specifies which parts the UMii for npc is put together.|``Dummy``|
  |``XlinkUser``|*String2*|?|``Weapon``|
  |``AnimationInfo``|*String2*|Specifies which AnimationInfo/.baniminfo file is used for the actor.|``Dummy``|
  |``ActorScale``|*Float*|Scale of actor presumable when spawned from .smubin. ?|``1``|
  
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
    
