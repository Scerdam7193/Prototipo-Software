# guardian-cache + session-handoff para Claude Code

Copia de respaldo del mod `guardian-cache` y de la skill `session-handoff`, para instalarlos en un computador local.

## Instalación (Mac / Linux)

Desde la raíz de este repositorio:

```sh
mkdir -p ~/.claude/mods ~/.claude/skills
cp -R claude-config/mods/guardian-cache ~/.claude/mods/
cp -R claude-config/skills/session-handoff ~/.claude/skills/
```

Luego, en `~/.claude/settings.json`, dentro de `"env"`, agrega la ruta absoluta del mod a `CLAUDE_CODE_PLUGIN_DIRS`.
Si la variable ya tiene rutas, súmala con `:`.

```json
{
  "env": {
    "CLAUDE_CODE_PLUGIN_DIRS": "/Users/<tu-usuario>/.claude/mods/guardian-cache"
  }
}
```

Reinicia Claude Code para que cargue el mod.
