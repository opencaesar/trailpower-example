---
tags:
  - operation/Capability
realizes:
involves: ["[[Sun]]"]
isImplementedBy:
isSupportedBy: "[[Trail Power]]"
specializes:
isSpecializedBy:
contains:
isContainedBy:
hasLabel:
hasDescription:
---
**Tags**: `= this.tags`
## Description
`INPUT[textArea:hasDescription]`
## Involves Entities
```dataview
List
FROM (#operation/Actor or #operation/Entity) and !"metadata/templates"
WHERE contains([[]].involves, file.link)
```
## Diagram
```dataviewjs
var s = ''
s += '```plantuml\n';
s += '@startuml\n'
s += 'left to right direction\n'
const capability = dv.current();
if (capability) {
	const name = capability.file.name
	const system = capability.isSupportedBy ? dv.page(capability.isSupportedBy) : null;
	if (system) {
		s += 'package "'+system.file.name+'" as '+system.file.name.replaceAll(" ", "_")+' {\n';
		s += 'usecase "'+ name+'" as ('+name.replaceAll(" ", "_")+')\n';
		s += '}\n';
	} else {
		s += 'usecase "'+ name+'" as ('+name.replaceAll(" ", "_")+')\n';
	}
	const actors = capability.involves?.map(i => dv.page(i)).filter(i => i.tags == "operation/Actor");
	actors?.forEach(i => s+= 'actor "'+ i.file.name+'" as '+i.file.name.replaceAll(" ", "_")+'\n')
	const entities = capability.involves?.map(i => dv.page(i)).filter(i => i.tags == "operation/Entity");
	entities?.forEach(i => s+= 'rectangle "'+ i.file.name+'" as '+i.file.name.replaceAll(" ", "_")+'\n')
	actors?.forEach(i => s += i.file.name.replaceAll(" ", "_")+" <-- ("+name.replaceAll(" ", "_")+')\n');
	entities?.forEach(i => s += '('+name.replaceAll(" ", "_")+") --> "+i.file.name.replaceAll(" ", "_")+'\n');
} else {
	s += 'note "RELOAD PAGE" as N1\n'
}
s += '@enduml\n';
s += '```'
dv.paragraph(s);
```