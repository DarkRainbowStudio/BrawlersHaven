## 1.11.0a (November 2, 2022)
	• Rewrote the API
		○ Migrated from Flask to FastAPI
		○ Authentication now uses OAuth2 specification
		○ WebSocket support
	• Implemented notifications
		○ Added a notifications button in the multiplayer menu. It animates when the player has notifications.
		○ Implemented the notifications menu
		○ Implemented notification alert widget
	• Implemented friends
		○ Implemented friends menu. When the player highlights a particular friend, their brawlers are displayed back.
		○ Implemented add friends menu. Allows the player to search for another player by username and send a friend request.
		○ Implemented friend requests. If the receiving player is online, they will get a notification. The receiving player can accept or decline the friend request.
	• Two new armor sets: the Leather set and the Hero set
	• Improved controller support
	• Updated Pause menu
	• The Characters button in the multiplayer menu has been renamed to the Brawlers button and is labeled with a special animated icon that displays back a representation of the player's brawlers
	• Improved attacking and rolling animations


## 1.10.0a (August 10, 2022)
	• A server build is now included with alpha releases. Alpha testers can execute a server and connect clients to it.
	• Moved a large portion of functionality from Blueprints to C++
	• Repositioned the menu pawn (which is what the player possesses when they are using the main menu)
	• Implemented attacking
	• Implemented death
	• Implemented target-lock
	• Reworked the character selector to organize the characters in a rotating carousel as opposed to a straight line

## 1.9.0a (June 1, 2022)
	• Migrated the project to Unreal Engine 5
	• Implemented a new UI with controller support (some functionality is incomplete)
	• Implemented character creation and selection. Accounts can have up to 5 characters.
	• Implemented loadout menu. Each character has 5 loadouts to customize.
	• Implemented weapon building. Weapons are broken into parts that players can customize.
	• Implemented armor selection
	• Implemented blocking
	• Implemented weapon two-handing
	• Reworked the database tables to optimize data storage
	• Reworked the API to improve data transferring and updating techniques
	• Created a new demo level with a test landscape to use while implementing basic mechanics
	• Moved the Tower model into the new demo level
	• Modeled a Mortuary building and placed it in the new demo level
	• Modeled more parts for the Battle Axe
	• Modeled a Claymore sword
	• Modeled the first shield

## 1.8.0a (March 21, 2021)
	• Fixed network syncing issues for rolling, attacking, weapon switching, and handedness.
	• Successfully built a server executable of Brawler's Haven and was able to connect two computers to the same session.
	• Shifted main menu elements leftward.
	• Retextured the Battle Axe and the Halberd
	• Purchased brawlershaven.com
	• Created a database to store player account data
	• Created an API server on a remote machine to handle account management and database operations.

## 1.7.0a (March 6, 2021)
	• Remodeled the tower
	• Remodeled and retextured the Estoc.  Other weapons will also get a retexture for their defaults.
	• Created a better rig for the brawler model to ease animating
	• Reanimated all actions with the improved rig
	• Reorganized weapon model files and how their texturing work
	• Optimized some models that were higher poly than they needed to be
	• Added the first attack animation: the Estoc jab.  Yield the Estoc and try attacking by clicking left mouse. 
	• Added a weapon selector accessible by pressing tab.  This menu will only exist in the demo level as the player will not normally be able to switch between all the weapons in the game.
	• Made it so that rolling occurs in the direction of the player's input (if input is present).

## 1.6.0a (December 16, 2020)
	• Added health and stamina bars.  The stamina bar is functional and depletes when sprinting or rolling.  It replenishes automatically.
	• Added texture to the tower (likely to change down the line)
	• Added a main menu
	• Added an options menu with a single option to change handedness
	• Added a pause menu

## 1.5.0a (December 2, 2020)
	• Reworked how the character's weapon and armor is spawned and handled
	• Brawlers, armor, and weapons now have a weight associated with them
	• New weapons: Introducing the Club, Estoc, Halberd, Katana, Longsword, and Sabre
	• Temporarily added more opposing brawlers to hold the new weapons in this build
	• Implemented left handedness
	• Implemented rolling which has replaced the jump action
	• Implemented sprinting which can be enabled by holding left shift on a keyboard or by clicking the left thumbstick on a controller
	• Optimized the brawler base model
	• Setup function calls to work on a client-server model

## 1.4.0a (November 16, 2020)
	• Walking can be enabled for keyboard users by holding Left-Ctrl
	• Walking and jogging can both be engaged by moving a controller's left thumbstick. Move the thumbstick slightly to walk and fully to jog
	• Created animation for Walking w/Right-hand yield
	• Brawler movement acceleration is now instant
	• Fixed non-breaking error message when launching the game
	• Adjusted weapon scale to align better with 3D software
	• Gave the player green eyes while leaving the enemy with red eyes

## 1.3.0a (November 11, 2020)
	• Brawler can now hold a weapon
	• Brawler head is now interchangeable, allowing for helmets
	• Placeholder helmet and weapon are included in this build
	• Camera boom no longer draws back when another brawler is between the player and the player's camera
	• Fixed black sky on mobile
	• Brawler collision height has been adjusted

## 1.2.0a (November 5, 2020)
	• Removed the clouds from the sky (sky is black on mobile temporarily)
	• Removed the default environment models that were being provided by the engine and replaced it with a tower model
	• Set player spawn to the top of the tower
	• Added a static brawler model opposing the player at spawn

## 1.1.0a (November 2, 2020)
	• Added an idle animation for the brawler model
	• Added a way for correct animations to play at the proper times
	• Fixed camera boom not springing in at the correct times

## 1.0.0a (November 2, 2020)
	• This release serves as the first versioning tag for this software. It is labeled as x.x.xa because it is not feature-complete, so therefore it is considered in the alpha stage. The following points briefly cover the features currently implemented:
		○ A template character model with animations for walking and jogging
		○ The character model is properly shaded and reflects the target art-style
		○ The player can control the character model.  There's movement, camera view rotation, and jumping.
		○ The only animation that plays is the jogging animation. There are no animation transitions currently. While other animations exist, you cannot view them in this build.
		○ Intentional camera speed lag and rotation lag enabled
		○ The level that the player spawns in is provided by Unreal Engine and is temporary
