# **There is no "basic" or "custom" AI. There is only ThothAI.** #
<a href='http://www.youtube.com/watch?feature=player_embedded&v=6ylXV8VvBes' target='_blank'><img src='http://img.youtube.com/vi/6ylXV8VvBes/0.jpg' width='425' height=344 /></a>

(8/9/2013)
you can download it here: https://hotfile.com/dl/238718757/51e4e24/Thoth_AI_6.5.rar.html
probably fixed a "beeper" error that somehow got left in.
thousands of downloads and no donations ever. haha. I'm sure you guys can understand why bugfixes were not at the top of my todo list :P

[![](https://www.paypalobjects.com/en_US/i/btn/btn_donate_LG.gif)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=9DUWXG9GFHGEJ)

## INTRODUCTION ##
If you want to take your homunculus or mercenary to PvP, Battlegrounds, or War of Emperium, ThothAI is the only choice. no other AI is capable of sorting enemies from friends in an effective manner. even though ThothAI records more details than other AI's and has more features, it tends to be faster because it actually preprocesses and stores this information instead of processing it every time it may possibly be needed. the complicated checks on whether or not someone is an enemy or not are only done once, and processing is not wasted on actors that you will not even be able to attack at all <sup>cough</sup> WoE Flags <sup>cough</sup>.

ThothAI also has many other features, such as:
  * attempts to interrupt enemy spellcasts
  * manually targeting a player can set them as a friend, ignore, or other behavior
  * Homunculus can attack marine spheres once and only once to launch them quickly
  * Homunculus and mercenary will attempt to protect each other
  * multiclient support (does not work when saving enemy list to disk)
  * attempts to decloak enemies with AOE if they cloak near you, based on last known position
  * Will "dance attack" toward the enemy making it difficult to run away
  * can be set to always attack or ignore specific players (based on account IDs)
  * will never break sleep status effect
  * superior sprite stacking ability (to make you hard to click)
  * MVP and monster kiting
  * ks detection, manually attacking will override
  * bow mercenaries can lay traps quickly in various formations
  * can instantly set everyone onscreen as an ally, or erase the enemy/ally list completely with manual commands
  * mercenaries will attempt to detect status effects and cure them based on owner action
  * fast config switching ingame
  * a complete feature list would be quite massive... for more complete information, see the readme and notes in the relevant config files.

  1. note that ThothAI may not work or may behave strangely on official servers. I have not had the opportunity to test it on these servers.
  1. Homunculus S is not supported. once again, I have not had the opportunity to test it. private server homun S remains bugridden last I knew
  1. there is currently no Graphical interface for the config files, as editing the text files was all I ever needed. I've not been given much outside motivation to make one either :P

### Why was this AI created? ###
I originally created ThothAI to address the problem of PvP friend or foe recognition for mercenaries while playing my gunslinger "The Smoking Nun". these problems stem from a fundamental problem in Gravity's AI implementation and the IsMonster function, which is supposed to tell you who your enemies are. while they should fix this and it would address the problems with other AIs, its been several years and I'm not holding my breath.

the workaround I devised is AI will cycle through possible targets onscreen, and if it is not busy with an enemy will cycle through a list and attempt to attack ALL of them until an enemy is confirmed. this method is especially effective with ranged attacks like caprice or bow mercenaries. it will then add them to a list of known enemies, and can save this list to disk. other checks based on owner/ally/enemy behavior are used as well.

over a period of several months it became an obsession of mine, to add more features and  to fill the gaping hole of AI capability within RO. when my AI grew powerful, the GMs of that server responded by completely removing mercenaries from WoE and Battlegrounds >.< . _With this public release, the playing field is now leveled for all._

I hope this AI will bring new possibilities to an old game for others, as it did for me.