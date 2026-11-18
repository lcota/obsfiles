fields:

  lead:
    type: MultiFile

  sponsor:
    type: MultiFile

  teams:
    type: MultiFile

  platforms:
    type: MultiFile

  desks:
    type: MultiFile

  people:
    type: MultiFile

  priority:
    type: Select
    options:
      - Low
      - Medium
      - High
      - Critical

  status:
    type: Select
    options:
      - Discovery
      - Planning
      - Active
      - Stabilization
      - Complete
