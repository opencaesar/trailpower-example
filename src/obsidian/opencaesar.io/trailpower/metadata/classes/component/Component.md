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
- name: contains
  type: MultiFile
  options:
    dvQueryString: "dv.pages('#component/Component or #component/System and !\"metadata/templates\"')"
  path: ""
  id: f899675353
- name: isContainedBy
  type: File
  options:
    dvQueryString: "dv.pages('#component/Component or #component/System and !\"metadata/templates\"')"
  path: ""
  id: f2049090498
- name: specializes
  type: MultiFile
  options:
    dvQueryString: "dv.pages('#component/Component or #component/System and !\"metadata/templates\"')"
  path: ""
  id: f807053698
- name: isSpecializedBy
  type: MultiFile
  options:
    dvQueryString: "dv.pages('#component/Component or #component/System and !\"metadata/templates\"')"
  path: ""
  id: f1607020784
- name: satisfies
  type: MultiFile
  options:
    dvQueryString: "dv.pages('#requirement/Requirement and !\"metadata/templates\"')"
  path: ""
  id: f930089183
- name: performs
  type: MultiFile
  options:
    dvQueryString: "dv.pages('#function/Function and !\"metadata/templates\"')"
  path: ""
  id: f921764975
- name: presents
  type: MultiFile
  options:
    dvQueryString: "dv.pages('#component/Interface and !\"metadata/templates\"')"
  path: ""
  id: f1775897362
- name: hasDescription
  type: Input
  path: ""
  id: f1940749968
---