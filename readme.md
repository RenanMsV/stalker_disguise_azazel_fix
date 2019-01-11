Outfit Disguise + Azazel Fix/Configs for Vanilla CoC 1.4.22

strelocc, sariskhan, RenanMsV

This mod is only for Vanilla CoC 1.4.22.
This is just a fix to use with CoC Azazel Mode.

You can use this mod to loot outfits from stalkers: https://www.moddb.com/mods/call-of-chernobyl/addons/outfit-loot-vanilla-coc-1422-fully-configurable

How to install:
	Copy and replace this mod's gamedata folder into your game's gamedata folder.

Using this Outfit Disguise + Azazel Mod you can:

Disguise:

	Disguise yourself as another faction (Even monolith, or loner)
	There was a glitch playing Azazel that makes your default faction freeze. So if you first spawned as a Monolith and died, even if you respawned as a loner everyone will still assume you're a Monolith guy, you wont notice that glitch until you get naked (this kind of a game breaking glitch, you can live with that, but it will piss you later).

Azazel: 
	
	You can now change some of the Azazel configurations editing the file Gamedata/configs/azazel_customizable.ltx
	Change Azazel configs such as how many money you get when respawning, fix bleeding and radiation glitches, disable Azazel animations between changing to a new character and more!

	You can enable bleeding and radiation fix.
	You can disable the transition animation.
	You can change the invulnerable time after the transition to a new character.
	You can change if you want to
		Get more money when you die (vanilla azazel system, you keep your money and receive 2000 RU more when respawning),
		Or You want to lose all your money when you die (hardcore huh? you will respawn with around 500 RU, about the same as a new game),
		Or if you want to get the money that your new character had (about 5000 RU)

Azazel Config file:
	```
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

