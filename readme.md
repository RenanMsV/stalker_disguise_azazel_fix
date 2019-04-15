Outfit Disguise + Azazel Fix/Configs for Vanilla CoC 1.4.22

strelocc, sariskhan, RenanMsV

This mod is only for Vanilla CoC 1.4.22.

This is just an improved version with many fixes to use the disguise mod with vanilla CoC Azazel Mode.


Do you ever wanted to use the disguise mod in Azazel mode without it glitching out? You can! (fixed glitch where your faction becomes freezed and never changes)

Do you ever wanted to disguise as Monolith and finish the game faster? You can!

Do you ever wanted to fix the Azazel radiation / bleeding? Or remove the transition animation? You can!

Do you ever wanted play HARD and LOSE your money when dying and start all over again? You can! (vanilla azazel gives you RU2000 when you die)

And many more!

You can use this mod to loot outfits from stalkers: https://www.moddb.com/mods/call-of-chernobyl/addons/outfit-loot-vanilla-coc-1422-fully-configurable

How to install:

* Copy and replace this mod's gamedata folder into your game's gamedata folder.
* Edit the config file as you like.
* Note: You can use the Azazel fix mod alone, but to run this version of Disguise mod the Azazel fix mod is required.

Using this Outfit Disguise + Azazel Mod you can:

Disguise:

* Disguise yourself as another faction (Even monolith, or loner)
* Fix a glitch playing Azazel that makes your default faction freeze. So if you first spawned as a Monolith and died, even if you respawned as a loner everyone will still assume you're a Monolith guy, you wont notice that glitch until you get naked (this is a kind of game breaking glitch, you can live with that, but it will bother you later).
* Change settings such (editing the file Gamedata/configs/disguise_customizable.ltx) as outfit condition, time to be suspected, or which outfit is from which faction.
* Add outfits or factions from mods.

Azazel Config file:

```ini

; Disguise Custom config file. Setup as you like.
[disguise_cfg]
;	time you need to be hidden (not seen by any npc) before changing outfit to make the disguise effective, 100 means roughly 10 seconds
	time_to_forget = 100
;	minimum condition for an outfit to work as disguise
;	set to 0 to not consider outfit condition, if you want only mint condition outfits to work set to 0.99 and not 1 because condition can never be exactly 1
	min_condition = 0.25
;	minimum condition for an helmet to reduce suspicion buildup
;	set to 0 to not consider helmet condition, if you want only mint condition helmets to work set to 0.99 and not 1 because condition can never be exactly 1
	min_condition_h = 0.25
;	distance within npc will start doubting the disguise (if they are seeing you)
;	5 = 1 wood box width
	discovery_distance = 25
;	how much time it takes to be discovered when in view, 100 is roughly 1 minute with uncovered face
	suspicion_limit = 100
;	debug messages? for developers
	debugMessages = false
;
[outfits]
;	Here you can change or add new outfits (from mods) or new factions (from mods) to the disguise system.
;	outfit_ = faction
	specops_ = army ; army
	military_ = army
	bandit_ = bandit ; bandit
	trenchcoat_ = bandit
	banditmerc_	 = bandit
	cs_ = csky ; clear sky
	svoboda_ = freedom ; freedom
	ecolog_ = ecolog ; ecologists
	dolg_ = dolg ; duty
	merc_ = killer ; mercenary
	monolith_ = monolith ; monolith
	stalker_ = stalker ; loner
	scientific_ = stalker
	exo_ = stalker
	novice_ = stalker

```

Azazel:

*  You can now change some of the Azazel settings editing the file Gamedata/configs/azazel_customizable.ltx
*  Change Azazel settings such as how many money you get when respawning, fix bleeding and radiation glitches, disable Azazel animations between changing to a new character and more!
*  You can enable/disable bleeding, hunger, and radiation fix.
*  You can disable the transition animation.
*  You can change the invulnerable time after the transition to a new character.
*  Get more money when you die (vanilla azazel system, you keep your money and receive 2000 RU more when respawning),
*  Or you want to lose all your money when you die (hardcore huh? you will respawn with around 500 RU, about the same as a new game),
*  Or if you want to get the money that your new character had (about 5000 RU)


Azazel Config file:

```ini
; Azazel Customizable by RenanMsV for CoC 1.4.22
[azazel_config]
	fix_bleeding = true ; This will fix the bleeding, radiation, hunger glitch from default Azazel
	disable_animation = false ; This will remove the animation between the transition to a new person. Instant transition.
	invul_time = 3000 ; This will set the invulnerable_time between the transition to a new person. (so you dont get shot again instantly)
	debugMessages = false ; debug
[azazel_money]
	; Gain Money system will have a higher priority in case one or more are enabled at the same time.
	gain_money = false ; Enable default system that you get about 2000 RU when you die.
	lose_all_money = true ; Enable new system that you lose all your money when you die and respawn with about 500 RU (as a new game does). You cant get the money back
	stalker_money = false ; Enable new system that you will respawn with the NPC's money.
```
