## 1.11.0a
    • Improve damage calculation
    	○ Weapon parts need a power value, and weapons need to calculate total power from their parts.
    	○ Armor needs a protection value
    	○ Both players' stats need to be part of the calculation
    • Implement friends system
    	○ API functionality
    	○ Friends button in Multiplayer menu
    	○ Friends menu
    	○ Player search
    • Implement rolling invincibility
    • Finalize blocking implementation
    	○ Dampen/prevent damage from incoming attacks
    	○ Calculate the direction of the attacking player and ensure that they are within the block window
    	○ Drain the blocking player's stamina as they are attacked.
    	○ If stamina is depleted while blocking, they will stagger and blocking will fail temporarily
    • Shorten the distance that the player travels when rolling
    • Speed up the axe basic attack animations

## 1.12.0a
	• Implement player lobbies
		○ Make UI changes for player lobbies
		○ Implement inviting to lobbies
		○ Implement joining lobbies
		○ Implement lobby privacy controls
	• Finalize target-lock implementation
		○ Trace for a brawler list instead of just one and lock onto the nearest one
		○ Create functionality to allow target-lock switching
	• Create more axe attacks
		○ Create heavy attack
        ○ Create running attack
        
## 1.13.0a
    • Implement mantling/vaulting
    • Implement throwing knives
    	○ Create gameplay functionality
        ○ Work on items option in loadouts
