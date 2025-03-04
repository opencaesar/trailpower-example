---
version: "2.1"
limit: 20
mapWithTag: true
icon: move-up-right
tagNames:
filesPaths:
bookmarksGroups:
excludes:
extends:
savedViews: []
favoriteView:
fieldsOrder: []
fields:
- name: transmits
  type: File
  options:
    dvQueryString: "dv.pages('#datatype/CompositeType or #datatype/DataType or #datatype/PrimitiveType and !\"metadata/templates\"')"
  path: ""
  id: f557982257
- name: implements
  type: MultiFile
  options:
    dvQueryString: "dv.pages('#operation/Capability and !\"metadata/templates\"')"
  path: ""
  id: f1904620350
- name: hasDescription
  type: Input
  path: ""
  id: f1940749968
- name: hasSource
  type: MultiFile
  options:
    dvQueryString: "dv.pages('#function/OutputPin or #function/Pin or #function/InputPin or #function/Function and !\"metadata/templates\"')"
  path: ""
  id: f648214522
- name: hasTarget
  type: MultiFile
  options:
    dvQueryString: "dv.pages('#function/OutputPin or #function/Pin or #function/InputPin or #function/Function and !\"metadata/templates\"')"
  path: ""
  id: f648214523
---