# Delta2
Repository for my final submission for delta's task 2
1. Game Setup
1.1 Map & Environment
Top-down view: Players see the city from above, including roads, buildings, and open zones.
Procedural generation: A new city layout is created each game, keeping gameplay fresh and unpredictable.
1.2 Objective
Collect Keys: Found at random locations throughout the map.
Decrypt Data Shards: Keys can be used to decrypt locked shards present at the Central Hub.
Deliver to Base Station: Decrypted shards should be transported to the Base Station to boost system health.
Maintain System Health: System health depletes over time; delivering Shards keeps the AUREX (system) alive.
1.3 Data Shards & Keys
Random Key Placement: Keys should be placed at different randomized locations over the map.
Keys as Currency: Keys are used for decrypting Data Shards.
Shard Requirements: Each Shard requires a specific number of keys.
1.4 Movement Rules
Navigable Terrain: Movement is allowed on roads and open areas.
Blocked Structures: Buildings and certain obstacles cannot be crossed.
1.5 User Interface
Display necessary elements like system health, player health, number of keys, and shard, etc.
1.6 Win/Loss Conditions
Win: System Health reaches 100%.
Loss:
Player’s health drops to zero.
System Health falls below the critical limit and can't recover in time.
__________________________________________________________________________________________________________________________________________________________
Normal mode 
Unique Maps: A unique and playable map should be generated for every game session.
Maps are generated using tile setup with tile size varying according to the screen width. Doesnt have an infinite map and central hub and base stations are random
Tower Combat: Implement rotating surveillance towers as described in point 2.1.
Game Controls: Pause, resume, and reset options.
Local Progress Storage: Saves high scores via localStorage.
Combat System:
Players can shoot bullets.
These bullets follow the law of reflection, bouncing off surfaces at equal angles relative to the normal and gradually losing speed with each bounce.
Infinite ammunition (i.e., bullets).
The survillance towers can be destroyed by these bullets.
