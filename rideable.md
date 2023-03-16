|rideエンティティID|rideコンポーネントグループ|riderエンティティファミリー|
|:-|:-|:-|
|boat|minecraft:can_ride|(すべて)|
|boat||(すべて)|
|cat|minecraft:cat_wild|zombie|
|cave_spider|minecraft:spider_jockey|skeleton|
|cave_spider|minecraft:spider_stray_jockey|skeleton|
|cave_spider|minecraft:spider_wither_jockey|skeleton|
|cave_spider||zombie|
|chest_boat|minecraft:can_ride|(すべて)|
|chest_boat||(すべて)|
|chicken|minecraft:chicken_adult|zombie|
|cow||zombie|
|donkey|minecraft:donkey_wild|player, zombie|
|donkey|minecraft:donkey_tamed|player|
|hoglin|minecraft:hoglin_baby|piglin|
|horse|minecraft:horse_wild|player, zombie|
|horse|minecraft:horse_tamed|player|
|husk|minecraft:zombie_husk_adult|zombie|
|llama|minecraft:llama_wild|player|
|llama|minecraft:llama_tamed|player|
|minecart||(すべて)|
|mooshroom||zombie|
|mule|minecraft:mule_wild|player, zombie|
|mule|minecraft:mule_tamed|player|
|ocelot|minecraft:ocelot_wild|zombie|
|panda||zombie|
|pig|minecraft:pig_unsaddled|zombie|
|pig|minecraft:pig_saddled|player|
|player||parrot_tame|
|ravager||pillager, vindicator, evocation_illager|
|sheep|minecraft:rideable_sheared|zombie|
|sheep|minecraft:rideable_wooly|zombie|
|skeleton_horse|minecraft:skeleton_horse_r5_upgrade||
|skeleton_horse|minecraft:skeleton_horse_adult|player,skeleton,zombie|
|skeleton_horse||player,skeleton,zombie|
|spider|minecraft:spider_jockey|skeleton|
|spider|minecraft:spider_stray_jockey|skeleton|
|spider|minecraft:spider_wither_jockey|skeleton|
|spider||zombie|
|strider|minecraft:strider_saddled|player|
|strider|minecraft:strider_piglin_jockey|player, zombie_pigman|
|strider|minecraft:strider_parent_jockey|strider|
|trader_llama|minecraft:llama_wild|player|
|trader_llama|minecraft:llama_tamed|player|
|wolf|minecraft:wolf_angry|zombie|
|wolf|minecraft:wolf_wild|zombie|
|zombie|minecraft:zombie_adult|zombie|
|zombie_horse|minecraft:horse_adult|zombie|
|zombie_pigman|minecraft:pig_zombie_adult|zombie|
|zombie_villager|adult|zombie|
|zombie_villager_v2|adult|zombie|

---
## 雑な説明
下のエンティティ(乗られる方)をride、上のエンティティ(乗る方)をriderとする。  
`/ride`コマンドで乗せることができるエンティティの組み合わせは決まっている。  
rideのエンティティID・コンポーネントグループとriderのエンティティファミリーとの組み合わせが合えば使える。  
rideコンポーネントグループが空欄の場合、コンポーネントグループの制限がない。  

`behaviour_pack/entities/<rideentity>.json`内に`minecraft:entity.component_groups.<ridegroup>.minecraft:rideable`あるいは`minecraft:entity.components.minecraft:rideable`があればその上にエンティティを乗せることができる。  
前者は、rideがコンポーネントグループ`<ridegroup>`を持っているときのみ。  
後者は、コンポーネントグループに関係なくいつでも。  
`minecraft:rideable.family_types`があれば、riderのエンティティファミリーを制限する。  
なお、`<rideentity>`, `<ridegroup>`は任意の文字列。  
