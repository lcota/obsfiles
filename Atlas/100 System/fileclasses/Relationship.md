fields:

  person:
    type: MultiFile

  trust_level:
    type: Select
    options:
      - Low
      - Medium
      - High
      - Very High

  interaction_frequency:
    type: Select
    options:
      - Weekly
      - Biweekly
      - Monthly
      - Quarterly
      - Occasional

  domains:
    type: MultiSelect

  value_types:
    type: MultiSelect
    options:
      - historian
      - navigator
      - trusted-advisor
      - mentor
      - connector
      - architect
      - thought-partner
      - problem-solver

  introduced_by:
    type: MultiFile
