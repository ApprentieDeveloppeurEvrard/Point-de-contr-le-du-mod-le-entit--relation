## Entités

### Gymnase
- id_gymnase (PK)
- nom
- adresse
- téléphone

### Membre
- id_membre (PK)
- nom
- prénom
- adresse
- date_naissance
- sexe
- id_gymnase (FK)

### Coach
- id_coach (PK)
- nom
- prénom
- âge
- spécialité

### Séance
- id_seance (PK)
- type_sport
- horaire
- max_participants (fixé à 20)
- id_gymnase (FK)

## Relations

### Inscription (Membre ↔ Séance)
- id_membre (FK)
- id_seance (FK)
- Max 20 membres par séance

### Animation (Coach ↔ Séance)
- id_coach (FK)
- id_seance (FK)
- Max 2 coachs par séance
