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
- name: isAggregatedBy
  type: MultiFile
  options:
    dvQueryString: "dv.pages('#component/Path and !\"metadata/templates\"')"
  path: ""
  id: f2062132026
- name: hasDescription
  type: Input
  path: ""
  id: f1940749968
- name: hasSource
  type: MultiFile
  options:
    dvQueryString: "dv.pages('#component/Interface and !\"metadata/templates\"')"
  path: ""
  id: f1022251997
- name: hasTarget
  type: MultiFile
  options:
    dvQueryString: "dv.pages('#component/Interface and !\"metadata/templates\"')"
  path: ""
  id: f1022251998
---