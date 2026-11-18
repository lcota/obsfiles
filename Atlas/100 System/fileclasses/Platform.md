fields:

  owner_team:
    type: MultiFile

  desks:
    type: MultiFile

  projects:
    type: MultiFile

  people:
    type: MultiFile

  status:
    type: Select
    options:
      - active
      - planned
      - sunset
      - retired

  criticality:
    type: Select
    options:
      - Low
      - Medium
      - High
      - Critical
