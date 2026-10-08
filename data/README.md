# Données locales

Ces fichiers sont chargés en priorité (le serveur distant n'est utilisé qu'en secours) :

| Fichier | Obligatoire | Contenu |
|---|---|---|
| `ghosts.json` | oui | `{ "ghosts": [{ "ghost": "...", "name": "...", ... }], "evidence": { ... } }` |
| `maps.json` | non | liste de `{ "div_id", "file_url", "event_url" }` |
| `weekly.json` | non | défi hebdomadaire (`challenge`, `description`, `map`, `details`, ...) |
| `3d-models.json` | non | liste de modèles 3D |
| `event.json` | non | événement en cours (`{ "version": false }` pour aucun) |

Sans `ghosts.json`, le site ne peut pas démarrer : ces données ne sont pas incluses dans le dépôt d'origine.
