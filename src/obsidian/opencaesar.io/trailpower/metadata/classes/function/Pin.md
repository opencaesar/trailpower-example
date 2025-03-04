---
version: "2.1"
limit: 20
mapWithTag: true
icon: 
tagNames:
filesPaths:
bookmarksGroups:
excludes:
extends:
savedViews: []
favoriteView:
fieldsOrder: []
fields:
- name: isPinOf
  type: File
  options:
    dvQueryString: "dv.pages('#function/Function and !\"metadata/templates\"')"
  path: ""
  id: f124540047
- name: sendsTo
  type: MultiFile
  options:
    dvQueryString: "dv.pages('#function/OutputPin or #function/Pin or #function/InputPin or #function/Function and !\"metadata/templates\"')"
  path: ""
  id: f146799499
- name: receivesFrom
  type: MultiFile
  options:
    dvQueryString: "dv.pages('#function/OutputPin or #function/Pin or #function/InputPin or #function/Function and !\"metadata/templates\"')"
  path: ""
  id: f954936400
- name: hasDescription
  type: Input
  path: ""
  id: f1940749968
---