---
version: "2.1"
limit: 20
mapWithTag: true
icon: square-function
tagNames:
filesPaths:
bookmarksGroups:
excludes:
extends:
savedViews: []
favoriteView:
fieldsOrder: []
fields:
- name: hasPin
  type: MultiFile
  options:
    dvQueryString: "dv.pages('#function/OutputPin or #function/Pin or #function/InputPin and !\"metadata/templates\"')"
  path: ""
  id: f377942196
- name: hasInput
  type: MultiFile
  options:
    dvQueryString: "dv.pages('#function/InputPin and !\"metadata/templates\"')"
  path: ""
  id: f956365425
- name: hasOutput
  type: MultiFile
  options:
    dvQueryString: "dv.pages('#function/OutputPin and !\"metadata/templates\"')"
  path: ""
  id: f131096911
- name: isPerformedBy
  type: File
  options:
    dvQueryString: "dv.pages('#component/Component or #component/System or #operation/Entity or #operation/Actor and !\"metadata/templates\"')"
  path: ""
  id: f1457075858
- name: satisfies
  type: MultiFile
  options:
    dvQueryString: "dv.pages('#requirement/Requirement and !\"metadata/templates\"')"
  path: ""
  id: f930089183
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