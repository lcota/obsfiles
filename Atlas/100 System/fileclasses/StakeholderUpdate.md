fields:

  week:
    type: Input

  audience:
    type: MultiSelect

  related_people:
    type: MultiFile

  related_teams:
    type: MultiFile

  related_platforms:
    type: MultiFile

  related_projects:
    type: MultiFile

  source_meetings:
    type: MultiFile

  source_assessments:
    type: MultiFile

  themes:
    type: MultiSelect

  status:
    type: Select
    options:
      - Draft
      - Sent
      - Archived

  created:
    type: Date
