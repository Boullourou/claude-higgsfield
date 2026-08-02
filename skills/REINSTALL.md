# Réinstaller les skills dans une nouvelle conversation

## Commande unique (toutes les skills)
```bash
npx skills add higgsfield-ai/skills --all
npx skills add heygen-com/skills --all
npx skills add elevenlabs/skills --all
npx skills add heygen-com/hyperframes --all
```

## Skills custom (uploader manuellement depuis ce repo)
Les skills suivants sont dans /skills/ et doivent être uploadés via Paramètres → Skills → Upload :
- soul-character-studio
- talking-head-director
- b-roll-shot-planner
- kling-3-prompt-director

## Vérification
```bash
ls /.agents/skills/ | wc -l
# Doit afficher 45+
```
