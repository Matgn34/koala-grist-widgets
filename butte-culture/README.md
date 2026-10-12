# 🌱 Suivi butte de culture

**FR** · [EN below](#english)

Widget Grist de suivi d'une butte de culture en permaculture : schéma de la butte et du jardin, choix de la plante à semer ou planter, suivi des récoltes, calendrier, journal avec photos, rappels.

## Installation automatique

1. Dans Grist : **Ajouter une page → Ajouter un widget à la page → Personnalisé**, source : n'importe quelle table.
2. Panneau de droite : **URL personnalisée**, colle :
   ```
   https://matgn34.github.io/koala-grist-widgets/butte-culture/index.html
   ```
3. Accès : **Accès complet au document** (obligatoire pour créer les tables).

Au premier affichage, le widget crée tout seul :

| Table | Contenu |
|---|---|
| `Butte_Plantes` | Catalogue de plantes (semis, plantation, récolte, quantités pour 4 personnes, espacements) |
| `Butte_Emplacements` | Emplacements du schéma de la butte |
| `Butte_Suivi` | Journal : semé, planté, récolté, retiré, notes, photos |
| `Butte_Rappels` | Rappels |
| `Butte_Jardin` | Plan du jardin (terrains, maison, butte, arbres…) |
| `Butte_Config` | Réglages |

Les mises à jour du widget complètent les tables existantes sans effacer tes données.

## Onglets

Butte (schéma, cotes décochables) · Jardin (plan, glisser-déposer) · Calendrier · Journal (notes, photos) · Rappels (lien vers Todoist).

## Personnaliser

- **Rappels Todoist** : modèle de lien modifiable dans la table `Butte_Config`, clé `todoist_url` (variables `{texte}`, `{date}`, `{desc}`, `{butte}`).
- **Plantes** : modifie ou ajoute des lignes dans `Butte_Plantes`. Les espacements fournis sont des valeurs usuelles indicatives.
- **Emplacements** : mode édition sur le schéma pour déplacer, créer ou supprimer.

## Limites

- Les emplacements fournis correspondent à une butte de 3,45 m × 1,60 m orientée nord-sud ; adapte-les à la tienne.
- Le widget charge `grist-plugin-api.js` depuis `docs.getgrist.com`.

---

## English

Grist custom widget to track a permaculture raised bed (butte): bed and garden diagrams, sowing/planting choices, harvest tracking, calendar, photo journal, reminders.

**Install:** add a *Custom* widget, pick any table as source, set *Custom URL* to
`https://matgn34.github.io/koala-grist-widgets/butte-culture/index.html`, and grant **Full document access**.
On first load the widget creates its own tables (`Butte_Plantes`, `Butte_Emplacements`, `Butte_Suivi`, `Butte_Rappels`, `Butte_Jardin`, `Butte_Config`) with starter data. Updates only add missing columns and catalog entries; your data is never overwritten.

Licence: MIT.
