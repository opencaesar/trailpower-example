## Functions

`BUTTON[function-button]`

```meta-bind-button
style: primary
label: Add Function
id: function-button
hidden: true
action:
  type: templaterCreateNote
  templateFile: "methodology/templates/Function.md"
  folderPath: "opencaesar.io/trailpower/operational/functions"
  openNote: true
```
```dataviewjs
const {fieldModifier: f} = this.app.plugins.plugins["metadata-menu"].api;
dv.table(['Function', 'Performer'], 
	 dv.pages('')
		 .where(p => p.tags == 'Function')
		 .filter(p => !p.file.path.includes('classes'))
		 .filter(p => !p.file.path.includes('templates'))
		 .map(p => [ p.file.link, f(dv, p, "isPerformedBy", {options: {alwaysOn: true, showAddField: true, inFrontmatter: true}}) ])
)
```
## Exchanges

`BUTTON[exchange-button, item-button]`

```meta-bind-button
style: primary
label: Add Exchange
id: exchange-button
hidden: true
action:
  type: templaterCreateNote
  templateFile: "methodology/templates/Exchange.md"
  folderPath: "opencaesar.io/trailpower/operational/functions"
  openNote: true
```
```meta-bind-button
style: primary
label: Add Item
id: item-button
hidden: true
action:
  type: templaterCreateNote
  templateFile: "methodology/templates/Item.md"
  folderPath: "opencaesar.io/trailpower/operational/functions"
  openNote: true
```
```dataviewjs
const {fieldModifier: f} = this.app.plugins.plugins["metadata-menu"].api;
dv.table(['Exchange', 'From', 'To', 'Item'], 
	 dv.pages('')
		 .where(p => p.tags == 'Exchange')
		 .filter(p => !p.file.path.includes('classes'))
		 .filter(p => !p.file.path.includes('templates'))
		 .map(p => [ p.file.link, 
			 f(dv, p, "hasSource", {options: {alwaysOn: true, showAddField: true, inFrontmatter: true}}),
			 f(dv, p, "hasTarget", {options: {alwaysOn: true, showAddField: true, inFrontmatter: true}}),
			 f(dv, p, "conveys", {options: {alwaysOn: true, showAddField: true, inFrontmatter: true}})
		 ])
)
```
## Chains

`BUTTON[chain-button]`

```meta-bind-button
style: primary
label: Add Chain
id: chain-button
hidden: true
action:
  type: templaterCreateNote
  templateFile: "methodology/templates/Chain.md"
  folderPath: "opencaesar.io/trailpower/operational/functions"
  openNote: true
```
```meta-bind-button
style: primary
label: Add Item
id: item-button
hidden: true
action:
  type: templaterCreateNote
  templateFile: "methodology/templates/Item.md"
  folderPath: "opencaesar.io/trailpower/operational/functions"
  openNote: true
```
```dataviewjs
const {fieldModifier: f} = this.app.plugins.plugins["metadata-menu"].api;
dv.table(['Chain', 'Capability', 'Exchanges'], 
	 dv.pages('')
		 .where(p => p.tags == 'Chain')
		 .filter(p => !p.file.path.includes('classes'))
		 .filter(p => !p.file.path.includes('templates'))
		 .map(p => [ p.file.link, 
			 f(dv, p, "implements", {options: {alwaysOn: true, showAddField: true, inFrontmatter: true}}),
			 f(dv, p, "aggregates", {options: {alwaysOn: true, showAddField: true, inFrontmatter: true}})
		 ])
)
```

