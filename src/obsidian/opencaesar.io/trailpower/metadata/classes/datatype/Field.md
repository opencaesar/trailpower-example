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
- name: hasType
  type: File
  options:
    dvQueryString: "dv.pages('#datatype/CompositeType or #datatype/DataType or #datatype/PrimitiveType and !\"metadata/templates\"')"
  path: ""
  id: f2139501486
- name: isPropertyOf
  type: File
  options:
    dvQueryString: "dv.pages('#datatype/CompositeType and !\"metadata/templates\"')"
  path: ""
  id: f826690115
- name: hasDescription
  type: Input
  path: ""
  id: f1940749968
---