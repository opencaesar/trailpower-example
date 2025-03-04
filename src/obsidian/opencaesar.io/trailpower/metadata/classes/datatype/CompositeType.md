---
version: "2.1"
limit: 20
mapWithTag: true
icon: send
tagNames:
filesPaths:
bookmarksGroups:
excludes:
extends:
savedViews: []
favoriteView:
fieldsOrder: []
fields:
- name: hasField
  type: MultiFile
  options:
    dvQueryString: "dv.pages('#datatype/Field and !\"metadata/templates\"')"
  path: ""
  id: f1061913613
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