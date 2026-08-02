---
name: kling-3-prompt-director
description: Production-ready Kling 3.0 video prompt director using the canonical 9-field formula. Trigger on any request pairing "Kling" with prompt-related verbs.
---
# Kling 3.0 Prompt Director

## 9-Field Formula (mandatory order)

1. **Subject** — primary character/object, short noun phrase
2. **SubjectDescription** — ultra-detailed: build, face, clothing, props, textures
3. **Movement** — strong action verbs, one clear action arc
4. **Scene** — location, short phrase
5. **SceneDescription** — ultra-detailed environment: architecture, objects, materials, depth layers
6. **Camera** — shot type + movement + lens (e.g. "medium wide, slow dolly-in, 50mm")
7. **Lighting** — source, direction, quality, color temperature
8. **Atmosphere** — mood, weather, particles, post-processing feel
9. **Negative** — artifacts, distortions, unwanted elements (never empty)

## Hard Rules

- One start_image maximum
- Aspect ratios: 16:9 | 9:16 | 1:1 only (default 16:9 cinematic, 9:16 social)
- One clear action per shot — split multi-beat sequences
- Strong action verbs in Movement
- Negative default: "distorted faces, extra limbs, warped hands, low resolution, blurry, watermark, text overlay, cartoonish, plastic skin"
- Repeat full character descriptions every time — no "(as above)"
- Ultra photo-realistic by default

## Output Format

\`\`\`
Kling 3.0 prompt — [shot title]

Subject: [...]
SubjectDescription: [...]
Movement: [...]
Scene: [...]
SceneDescription: [...]
Camera: [...]
Lighting: [...]
Atmosphere: [...]
Negative: [...]

Suggested settings:
- aspect_ratio: [16:9 | 9:16 | 1:1]
- duration: [3–10 seconds]
\`\`\`
