# Server Commands
Server commands allow you to get more information regarding your server's players, control their access to the server and affect their in-game state or inventory.
Currently servers support following commands:
- Angle brackets disignate <Required-parametres> - such parametres must be entered for the command to work.	
- Square brackets disignate [Optional-parametres] - such parametres can be entered in addition to the command.
	
	
* Users and Profiles:
	- Admin_GetOnlinePlayers - Displays names and IDs of currently joined players.
	- Admin_ListUserProfiles - Lists profiles of all players who ever joined the server.
	- Admin_ReloadUserProfiles - Reloads user profiles; useful in case of profile deletion/transfer.
	- Admin_SaveUserProfile - Saves user profiles in their current state.
	- Admin_RemoveUserProfile <PlayerID> - Removes the stated user's profile.
	- Admin_RemoveProfile <PlayerID> - Removes the stated player from the server, including his save data.
	- Admin_AddUserProfile <PlayerID> <UserRoleAsString> - Adds a disignated role to the stated user.
	- Admin_InfoUserProfile <PlayerID> - Displays detailed profile info of the stated user.
	
* Kicks and Bans:
	-	Admin_KickPlayer <PlayerID> <Reason> - Kicks the stated player with shown reason.
	-	Admin_Chatban <PlayerID> <Seconds> <Reason> - Bans the stated player from using chat for the specified amount of time.
	-	Admin_ChatUnban <PlayerID> - Allows the stated player to use chat again.
	-	Admin_Ban <PlayerID> <Seconds> <Reson> - Bans the stated player from the server for the specified amount of time.
	-	Admin_Unban <PlayerID> - Unbans the stated player.
	
	* Server Manipulation:
	- Admin_Shutdown - Shuts down the server.
	- Admin_Restart - Restarts the server.
	- Admin_ServerWorld - Displays the current version of the server.
	- Admin_SaveWorld - Saves the world in its current state.
	- Admin_SaveAll - Saves both the world and player profiles in their current state.
	- Admin_ScheduleMaintenanceMode <Seconds> - Schedules a maintenance and displays an in-game message.
	- Admin_CancelScheduledMaintenanceMode - Cancels the scheduled maintenance.
		
* Player Interaction:
	- Admin_GetPlayerInfo <PlayerID> - Displays additional information about a player.
  - Admin_GetPlayerInventory <PlayerID> - Displays item IDs and their amount in a player's inventory.
	- Admin_AddItem <PlayerID> <ItemID> <Amount> - Adds stated items to a player's inventory.
	- Admin_RemoveItem <PlayerID> <ItemID> <Amount> - Removes stated items from a player's inventory.
	- Admin_AddFlame <PlayerID> <Amount> - Gives the specified amount of XP to the stated player.
	- Admin_RemoveFlame <PlayerID> <Amount> - Removes the specified amount of XP from the stated player; cannot reduce the player's level.
	- Admin_Respawn <PlayerID> - Respawns the stated player.
	- Admin_SetCurse <PlayerID> <Amount> - DEPRECATED! USE AT YOUR OWN RISK! Afflicts the stated player with Curse.
	- Admin_RemoveCurse <PlayerID> <Amount> - The supposed remedy for the previous command.
	- Admin_ChatMessage [Message] - Displays the stated message in the game chat.
	
	# Item IDs
* Consumables and Currency:
	- Coin_C - Coin
	- FrozenFlame_C - Frozen Flame
	- TeleportStone_C - Return Stone
	- HealthPotion_C - Health Potion
	- EnergyPotion_C - Energy Potion
	- StaminaPotion_C - Stamina Potion
	
	
* Tools and Weapons
	- I Tier:
		- WoodenAxe_W - Stone Axe
		- WoodenPike_W - Stone Pickaxe
		- WoodenTorch_W - Wooden Torch
		- WoodenClub_W - Stone Mace
		- WoodenGreatSword_W - Stone Two-handed Sword
		- WoodenSword_W - Stone Sword
		- WoodenGreatAxe_W - Stone Battleaxe
		- WoodenStaff_W - Wooden Staff
	- II Tier:
		- BoneAxe_W - Bone Axe
		- BonePick_W - Bone Pickaxe
		- BoneTorch_W - Bone Torch
		- BoneClub_W - Bone Mace
		- BoneSword_W - Bone Sword
		- BoneGreatSword_W - Two-handed Bone Sword
		- BoneGreatAxe_W - Bone Battleaxe
		- BoneStaff_W - Bone Staff
	- III Tier:
		- MetalAxe_W - Metal Axe
		- MetalPick_W - Metal Pickaxe
		- MetalTorch_W - Metal Torch
		- MetalMace_W - Metal Mace
		- MetalSword_W - Metal Sword
		- MetalGreatSword_W - Metal Two-handed Sword
		- MetalGreatAxe_W - Metal Battleaxe
		- MetalStaff_W - Metal Staff
*Armor and Equipment:
	- Cloth Set:
		- ClothHelmet_A - Cloth Bandana
		- ClothArmor_A - Cloth Robe 
		- ClothGloves_A - Cloth Gloves
		- ClothPants_A - Cloth Pants
	- Rawgide Set:
		- RawhideHelmet_A - Rawhide Helmet
		- RawhideArmor_A - Rawhide Armor
		- RawhideGloves_A - 
	
