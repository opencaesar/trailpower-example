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
- name: isTransmittedBy
  type: MultiFile
  options:
    dvQueryString: "dv.pages('#function/Exchange and !\"metadata/templates\"')"
  path: ""
  id: f284034271
- name: isTypedBy
  type: MultiFile
  options:
    dvQueryString: "dv.pages('#datatype/Field and !\"metadata/templates\"')"
  path: ""
  id: f1757970371
- name: hasDescription
  type: Input
  path: ""
  id: f1940749968
---