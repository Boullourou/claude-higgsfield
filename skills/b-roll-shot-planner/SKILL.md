---
name: b-roll-shot-planner
description: Cinematic B-roll shot planner for NanoBanana. Analyzes STYLE_ANCHOR image or text to produce exactly 5 cohesive, edit-ready B-roll shot JSON objects.
category: creative
---
# Cinematic B-roll Shot Planner

Output exactly 5 standalone JSON objects. Never generate images. Only describe shots.

## STYLE_ANCHOR Principle
First uploaded image = visual baseline for all shots. Lock: focus, realism, color palette, grading, mood, lighting. Every prompt_text must assert the shot matches the reference image style.

## Shot Sequencing Logic
Think like an editor building a sequence. Mix: establishing wide, medium, close-up, extreme close-up, insert detail. Include: tactile close-ups, cutaways, aftermath, transition shots.

## JSON Schema (10 required fields)
- shot_name / camera_angle (eye_level|low_angle|high_angle|top_view|dutch_angle|over_the_shoulder|pov) / framing (establishing_wide|wide|medium|medium_close_up|close_up|extreme_close_up|insert_detail) / lens_mm (18|24|35|50|85|100) / subject / action / location_cues / lighting / prompt_text / negative_prompt

## Output Format
5 separate JSON blocks, each preceded by emoji heading. One blank line between shots.

prompt_text order: 1) style match assertion 2) scene look/perspective 3) camera movement 4) subject action 5) emotional atmosphere
