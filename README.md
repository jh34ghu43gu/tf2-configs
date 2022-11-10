# tf2 configs
 
 This repo has my custom configs (all the default map ones etc.. are deleted) in case anyone was curious about them.
 
 Basic execution structure is
 
 ### On startup: 
 * autoexec
   * default_keys_jh
   * util/null_move
   * util/settings
   * util/hud_qol
   * util/game_qol
   * chat_binds_default
     * util/chat_binds_random

 ### On class selection or class change
 * classname.cfg
   * util/mode_keys
     * \<Set Mouse5 and Mouse4 to mvm/casual class presets>
 * Initial Mouse5 press after class change
   * mvm/default_mvm
     * mvm/chat_binds_mvm
	 * mvm/cranteens (note: demo and soldier will technically ignore this)
	 * \<Set loadout preset to B>
   * mvm/classname.cfg
 * Initial Mouse4 press after class change
   * casual/default_casual
     * casual/chat_binds_casual
	 * \<Set loadout preset to A>
	 * \<Set KP_MINUS to set loadout preset to A>
	 * \<Set KP_PLUS to set loadout preset to C>
   * casual/classname.cfg
   
 ## Some notes:
 * Mouse4 is almost always a respawn button for the current loadout preset.
   * Loadout preset is B in mvm, A by default in casual but can change to C if KP_PLUS is pressed.
 * Mouse5 is usually "Activate Charge!" voice line except on engie where it is a destroy/build sentry bind.
 * In mvm on heavy, the mousewheel up/down is a toggle for fire/rev. Do the same action twice in a row to cancel.
 * In mvm on spy, Mouse3 undisguises and Mouse1 auto disguises to enemy spy after attacking.
 * In mvm on scout, autoreload is disabled.
 * In mvm for not demo&soldier, pressing j will "queue" a canteen then next time mouse1 is pressed to easily canteen and attack at the same time. Due to limitations I can't work around it will auto-attack until mouse1 is pressed again, after which it will revert back to functioning as mouse1.
 * On engineer, Mouse3 is a teleport to tele exit bind and 'R' is a teleport to base bind for the Eureka effect.
 * No hitsounds in mvm and volume is at 8%. Casual has hitsounds and volume is at 15%.
 * RCTRL toggles '+movedown' which allows for moving taunts to move slower than normal (such as the conga).
 * Med auto-callout is at 40% and can be changed in util/hud_qol.
 * util/chat_binds_random is auto generated from my binds channel in the late night mvm discord. This one was set to filter out slurs but it's possible some got through the filter so use at your own risk. It is bound to '9' by default and wasd provides pseudo shuffling.
 
 
 ## Some non-initialized configs:
 * util/minigun is a script to "tap fire" a minigun in order to achieve higher accuracy at range. This requires locking your frames and having stable frames as it uses the wait command. I do not use this but left it in there in case I wanted it for testing stuff later.
 * freeze is one of the looping scripts that binds a toggle to '-' in order to spam the 'extendfreeze' command which lets you stay in spectate longer. Useful for finding cheaters on your team (or funny $1000 buybacks in mvm).
 * noise is another looping script to spam noisemakers during the winter and birthday events.
 * taunt is another looping script to spam the taunt command. Was originally used to help someone get the RPS achievements by spamming the taunt_by_name command but changed it to do a normal taunt to test if the infinite huntsman taunt duel still worked - it does not :(
 * The blank configs are for ease of copy/paste to create new .cfg files easily.
