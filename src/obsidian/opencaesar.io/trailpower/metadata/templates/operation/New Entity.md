---
tags:
  - operation/Entity
specializes:
isSpecializedBy:
performs:
presents:
inInvolvedIn:
hasDescription:
---
**Tags**: `= this.tags`
## Description
`INPUT[textArea:hasDescription]`
## Involved In Capabilities
```dataview
List
FROM #operation/Capability and !"metadata/templates"
WHERE contains(involves, [[]])
```