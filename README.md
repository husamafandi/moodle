# Moodle Boost Union – Externes SCSS (Moodle 4.5)

Dieses Repo enthält zwei SCSS-Dateien für **Boost Union** als externe Quelle:

- `extscss-pre.scss` → **Pre-SCSS**: Variablen/Maps/Mixins (kompiliert alleine; ideal wenn Validierung aktiv ist)
- `extscss-post.scss` → **Post-SCSS**: Eigentliche Styles für Moodle/Boost Union

## Einbindung in Moodle (Theme Boost Union)

1. **Quelle wählen**
   - `theme_boost_union | extscsssource` → *Privates Github-Repository* **oder** *Öffentliche URL*

2. **Privates GitHub verwenden**
   - `theme_boost_union | extscssgithubtoken` → Personal Access Token (nur Lesen)
   - `theme_boost_union | extscssgithubuser` → Besitzer:in/Organisation (z. B. `dein-orgname`)
   - `theme_boost_union | extscssgithubrepo` → Repo-Name (z. B. `moodle-boost-union-extscss`)
   - `theme_boost_union | extscssgithubprefilepath` → `/extscss-pre.scss`
   - `theme_boost_union | extscssgithubpostfilepath` → `/extscss-post.scss`

3. **Validierung**
   - Aktiv lassen, solange Pre-SCSS keine Moodle/Bootstrap-Variablen importiert.
   - Wenn du Core-Variablen in externem SCSS brauchst → Validierung deaktivieren und selbst prüfen.

4. **Task (optional)**
   - `theme_boost_union\task\purge_cache` zeitgesteuert aktivieren, um Code regelmäßig neu zu ziehen.
   - Nach Änderungen: *Website-Administration → Entwicklung → Alle Caches leeren*.

## Anpassung
Passe Farben/Typo in `extscss-pre.scss` an (`$brand-…` Variablen). Die Post-Styles nutzen diese Werte automatisch.
