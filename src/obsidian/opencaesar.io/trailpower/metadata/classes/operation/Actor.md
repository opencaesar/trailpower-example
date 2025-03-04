---
version: "2.1"
limit: 20
mapWithTag: true
icon: user
tagNames:
filesPaths:
bookmarksGroups:
excludes:
extends:
savedViews: []
favoriteView:
fieldsOrder: []
fields:
- name: specializes
  type: MultiFile
  options:
    dvQueryString: "dv.pages('#operation/Actor and !\"metadata/templates\"')"
  path: ""
  id: f807053698
- name: isSpecializedBy
  type: MultiFile
  options:
    dvQueryString: "dv.pages('#operation/Actor and !\"metadata/templates\"')"
  path: ""
  id: f1607020784
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
- name: inInvolvedIn
  type: MultiFile
  options:
    dvQueryString: "dv.pages('#operation/Capability and !\"metadata/templates\"')"
  path: ""
  id: f2139266166
- name: hasDescription
  type: Input
  path: ""
  id: f1940749968
---