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
- name: isPursuedBy
  type: File
  options:
    dvQueryString: "dv.pages('#operation/Mission and !\"metadata/templates\"')"
  path: ""
  id: f153443333
- name: isRealizedBy
  type: File
  options:
    dvQueryString: "dv.pages('#operation/Capability and !\"metadata/templates\"')"
  path: ""
  id: f2021854618
- name: contains
  type: MultiFile
  options:
    dvQueryString: "dv.pages('#operation/Objective and !\"metadata/templates\"')"
  path: ""
  id: f899675353
- name: isContainedBy
  type: File
  options:
    dvQueryString: "dv.pages('#operation/Objective and !\"metadata/templates\"')"
  path: ""
  id: f2049090498
- name: hasDescription
  type: Input
  path: ""
  id: f1940749968
---