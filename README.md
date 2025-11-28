# LevelUpSystem

⚡ LevelManager – Trade-Off Based Progression System for Unity

A flexible and strategy-focused level-up system designed for Unity.
Perfect for RPG, survival, and progression-heavy action games that require meaningful upgrade choices rather than linear stat increases.

✨ Overview

LevelManager introduces a dynamic trade-off system:
every milestone level (e.g., every 50 levels), the player is presented with three upgrade cards, each offering a unique buff paired with a balancing nerf.

Instead of straightforward stat gains, the system forces strategic decisions, enhancing replayability and increasing player agency.
All milestone behaviors, stat changes, and XP scaling are fully customizable through the Unity Inspector.

🎮 Features
🃏 Trade-Off Upgrade Cards

When reaching milestone levels, the system displays 3 upgrade options:

Each card increases one stat (buff)

And reduces another stat (nerf)

Stats & amounts are fully configurable

Cards can be procedurally generated or manually defined

Perfect for builds like:

+10 Speed / -10 Max Health

+20 Jump Force / -20 Damage

+30 Damage / -30 Speed

📈 XP & Leveling System

A built-in progression system that handles:

XP gain

Required XP scaling (via multiplier)

Level-up detection

UI slider updates

XP requirements grow non-linearly, ensuring dynamic difficulty and long-term progression.

🎯 Milestone-Based Triggers

You can set:

Global milestones (e.g., every 50 levels)

Special handcrafted milestones (e.g., 50, 100, 150…)

Unique trade-off sets per milestone

The system automatically detects the correct milestone type and displays the appropriate cards.

🧬 Player Stat Integration

Supports default stats:

Move Speed

Jump Force

Max Health

Damage

Developers can easily expand the stat system through an enum.

Buffs and nerfs are applied instantly and displayed live in the UI.

🌀 Procedural Option Generation

If no special milestone is defined:

Random buff stat

Random nerf stat

Level-scaled values

Risk tiers (Light / Medium / Heavy)

Ensures unique and replayable progression every run.

🖥 Animated UI

DOTween-powered card animations:

Panel smoothly scales in/out

Game pauses during selection

UI is clean, responsive, and player-friendly

📜 Inspector Breakdown
🔹 Level Settings
Field	Description
milestoneInterval	Level interval triggering card selection
xpRequired	XP to reach next level
xpMultiplier	Controls XP growth rate
currentLevel	Player's current level
🔹 Milestone Configurations
Field	Description
specializedMilestones	Custom card sets for specific levels
option1/2/3	The three trade-off cards presented to the player
🔹 Trade-Off Option
Field	Description
optionName	Card name (e.g., “Medium Risk”)
buffType	Stat to increase
buffAmount	Increase amount
nerfType	Stat to decrease
nerfAmount	Decrease amount
🔹 Player Stats
Field	Description
walkSpeed	Movement speed
jumpHeight	Jump force
maxHealth	Max HP
damage	Damage output
💡 Tips

Use LevelMultipliers to scale buff/nerf values smoothly.

Combine with an inventory or perk system for deeper builds.

Add rarity colors (Common / Rare / Epic) for advanced card variations.

Tune XP scaling early to match your game’s pace.

🔧 Requirements

Unity 2021.3 or newer

DOTween (for UI animation)

Works with URP / HDRP / Built-In
