---
tags:
  - Capability
involves:
  - "[[Charger]]"
  - "[[USB Device]]"
---
This capability allows using a [[Charger]] to charge a [[USB Device]].

```plantuml-svg
rectangle Charger
rectangle "USB Device" as USB_Device
usecase "Charge USB Device" as Charge_USB_Device

Charger -r-> Charge_USB_Device
USB_Device -l-> Charge_USB_Device

url of Charger is [[[Charger]]]
url of USB_Device is [[[USB Device]]]
url of Charge_USB_Device is [[[Charge USB Device]]]
```