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
- name: sendsTo
  type: MultiFile
  options:
    dvQueryString: "dv.pages('#component/Interface and !\"metadata/templates\"')"
  path: ""
  id: f1940737740
- name: receivesFrom
  type: MultiFile
  options:
    dvQueryString: "dv.pages('#component/Interface and !\"metadata/templates\"')"
  path: ""
  id: f688581408
- name: isPresentedBy
  type: File
  options:
    dvQueryString: "dv.pages('#component/Component or #component/System or #operation/Entity or #operation/Actor and !\"metadata/templates\"')"
  path: ""
  id: f660915526
- name: hasDescription
  type: Input
  path: ""
  id: f1940749968
---