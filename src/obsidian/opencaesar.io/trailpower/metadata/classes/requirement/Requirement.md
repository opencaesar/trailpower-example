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
- name: hasStatement
  type: Input
  path: ""
  id: f356338363
- name: hasRationale
  type: Input
  path: ""
  id: f1833707324
- name: hasConstraint
  type: MultiFile
  options:
    dvQueryString: "dv.pages('#requirement/Constraint and !\"metadata/templates\"')"
  path: ""
  id: f753162875
- name: isSatisfiedBy
  type: MultiFile
  options:
    dvQueryString: "dv.pages('#component/Component or #function/Function or #component/System and !\"metadata/templates\"')"
  path: ""
  id: f1410186665
- name: hasId
  type: Input
  path: ""
  id: f1710591086
- name: contains
  type: MultiFile
  options:
    dvQueryString: "dv.pages('#requirement/Requirement and !\"metadata/templates\"')"
  path: ""
  id: f899675353
- name: isContainedBy
  type: File
  options:
    dvQueryString: "dv.pages('#requirement/Requirement and !\"metadata/templates\"')"
  path: ""
  id: f2049090498
- name: refines
  type: MultiFile
  options:
    dvQueryString: "dv.pages('#requirement/Requirement and !\"metadata/templates\"')"
  path: ""
  id: f922871524
- name: isRefinedBy
  type: MultiFile
  options:
    dvQueryString: "dv.pages('#requirement/Requirement and !\"metadata/templates\"')"
  path: ""
  id: f13001549
- name: derives
  type: MultiFile
  options:
    dvQueryString: "dv.pages('#scenario/Scenario and !\"metadata/templates\"')"
  path: ""
  id: f1929661663
- name: isDrivenBy
  type: MultiFile
  options:
    dvQueryString: "dv.pages('#scenario/Scenario and !\"metadata/templates\"')"
  path: ""
  id: f1019009267
- name: hasDescription
  type: Input
  path: ""
  id: f1940749968
---