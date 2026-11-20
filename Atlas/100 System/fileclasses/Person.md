fields:

title:
	type: Input

position:
	type: Input

company:
  type: MultiFile

affiliation:
  type: Select
  options:
    - Employee
    - Contractor
    - Consultant
    - Vendor
    - Client
    - Former Employee

division:
  type: MultiFile

group:
  type: MultiFile

  team:
    type: MultiFile

  desks:
    type: MultiFile

  platforms:
    type: MultiFile

  projects:
    type: MultiFile

  roles:
    type: MultiSelect
    options:
      - connector
      - historian
      - navigator
      - trusted-advisor
      - architect
      - influencer
      - operator
      - sponsor
      - decision-maker
      - sme

  relationship_strength:
    type: Select
    options:
      - Weak
      - Developing
      - Strong
      - Trusted
      - Strategic

  knowledge_capital:
    type: Select
    options:
      - 1
      - 2
      - 3
      - 4
      - 5

  network_capital:
    type: Select
    options:
      - 1
      - 2
      - 3
      - 4
      - 5

  execution_capital:
    type: Select
    options:
      - 1
      - 2
      - 3
      - 4
      - 5

  navigation_value:
    type: Select
    options:
      - 1
      - 2
      - 3
      - 4
      - 5

  status:
    type: Select
    options:
      - active
      - inactive
      - historical
