fields:

  status:
    type: Select
    options:
      - Planned
      - Active
      - On Hold
      - Complete

  owner:
    type: MultiFile

  related_people:
    type: MultiFile

  related_teams:
    type: MultiFile

  related_platforms:
    type: MultiFile

  related_projects:
    type: MultiFile

  start_date:
    type: Date

  target_date:
    type: Date
