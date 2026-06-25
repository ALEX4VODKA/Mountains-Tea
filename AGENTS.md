# AGENTS.md

## Project Overview

This is a Godot 4 project called "Mountain Tea House".

It is a small 2D top-down pixel-art cozy exploration and shopkeeping game. The project focuses on beautiful scenery, calm atmosphere, simple collecting, simple crafting, and a small shopkeeping loop.

The goal is not to build a full commercial game. The goal is to create a small, playable 5 to 10 minute demo.

## Core Direction

- Engine: Godot 4
- Renderer: Compatibility
- Language: GDScript
- Style: 2D pixel art
- Camera: top-down
- Mood: scenic, warm, quiet, misty, nature-focused
- Theme: mountain tea house, forest, stone path, stream, warm lights

## Gameplay Loop

Wake up in the tea house  
→ explore nearby nature areas  
→ collect resources  
→ return to the tea house  
→ craft tea or simple goods  
→ sell to visitors  
→ sleep  
→ next day

## First Milestone

The first playable demo should include:

1. Player movement
2. Camera follow
3. One small map
4. A tea house area
5. Three collectible resources
6. A simple inventory
7. One simple crafting interaction
8. One simple selling interaction
9. Day/night transition
10. Sleep interaction to start the next day

## Initial Resources

Use these first resources:

- tea_leaves
- spring_water
- firewood

## Initial Recipe

The first recipe is:

tea_leaves + spring_water = simple_tea

## Initial Selling Rule

The player can sell:

- simple_tea

Selling simple_tea increases the player's money.

## Non-Goals

Do not add these in the first milestone unless explicitly requested:

- combat
- large story systems
- large open world maps
- complex NPC schedules
- complex dialogue trees
- skill trees
- equipment systems
- random dungeon generation
- multiplayer
- complex save systems
- oversized architecture

## Development Rules

- Keep every task small and focused.
- Prefer beginner-friendly, readable GDScript.
- Explain where each script should be attached.
- Use placeholder assets if real assets are missing.
- Do not over-engineer the project.
- Do not create unnecessary managers or abstractions.
- Do not add combat in the first milestone.
- Do not add complex RPG systems unless requested.
- Each feature should be easy to test inside Godot.

## Response Format After Each Task

After completing a task, respond with:

1. Changed files
2. What each file does
3. How to test in Godot
4. Possible next step

## Scene Organization

Prefer this structure:

- scenes/main/
- scenes/player/
- scenes/world/
- scenes/interactables/
- scenes/ui/
- scenes/npc/

## Script Organization

Prefer this structure:

- scripts/player/
- scripts/systems/
- scripts/interactables/
- scripts/ui/
- scripts/npc/

## Art Direction

Use pixel-art assets with strong natural scenery:

- trees
- grass
- stone paths
- mountain background
- stream
- wooden tea house
- warm lamps
- mist or fog
- cozy interior

Visual priority:

1. scenery quality
2. atmosphere
3. clarity
4. gameplay readability

Do not depend on rare wuxia-specific assets. Use general high-quality nature pixel-art assets first. Chinese or wuxia details can be added later through small props such as lanterns, tea tables, wooden signs, bamboo, stone roads, and warm window lights.
