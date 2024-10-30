## Capabilities

`BUTTON[capability-button, actor-button, entity-button]`

```meta-bind-button
style: primary
label: Add Actor
id: actor-button
hidden: true
action:
  type: templaterCreateNote
  templateFile: "methodology/templates/Actor.md"
  folderPath: "opencaesar.io/trailpower/operational/capabilities"
  openNote: true
```
```meta-bind-button
style: primary
label: Add Entity
id: entity-button
hidden: true
action:
  type: templaterCreateNote
  templateFile: "methodology/templates/Entity.md"
  folderPath: "opencaesar.io/trailpower/operational/capabilities"
  openNote: true
```
```meta-bind-button
style: primary
label: Add Capability
id: capability-button
hidden: true
action:
  type: templaterCreateNote
  templateFile: "methodology/templates/Capability.md"
  folderPath: "opencaesar.io/trailpower/operational/capabilities"
  openNote: true
```
```dataviewjs
const {fieldModifier: f} = this.app.plugins.plugins["metadata-menu"].api;

dv.table(['Capability', 'Involves'], 
	 dv.pages('')
		 .where(p => p.tags == 'Capability')
		 .filter(p => !p.file.path.includes('classes'))
		 .filter(p => !p.file.path.includes('templates'))
		 .map(p => [ p.file.link, f(dv, p, "involves", {options: {alwaysOn: true, showAddField: true, inFrontmatter: true}}) ])
)
```

## Overview

```plantuml-svg
left to right direction

	usecase "Disconnect to USB Device Cable" as Disconnect_USB_Device_Cable
	usecase "Connect to USB Device Cable" as Connect_to_USB_Device_Cable
	usecase "Provide 24h Visibility" as Provide_24h_Visibility
	usecase "Monitor Operation Remotely" as Monitor_Operation_Remotely
	usecase "Charge USB Device" as Charge_USB_Device

actor User [[User]]
actor Developer [[Developer]]

rectangle Charger [[Charger]]
rectangle "USB Device" as USB_Device [[USB Device]]

User <-- Disconnect_USB_Device_Cable
User <-- Connect_to_USB_Device_Cable
User <-- Provide_24h_Visibility

Developer <-- Monitor_Operation_Remotely
Developer <-- Charge_USB_Device

Disconnect_USB_Device_Cable --> Charger
Connect_to_USB_Device_Cable --> Charger
Provide_24h_Visibility --> Charger
Monitor_Operation_Remotely --> Charger

Disconnect_USB_Device_Cable --> USB_Device
Connect_to_USB_Device_Cable --> USB_Device
Charge_USB_Device --> USB_Device


```
