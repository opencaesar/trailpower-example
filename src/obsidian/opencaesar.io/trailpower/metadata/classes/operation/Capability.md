---
version: "2.1"
limit: 20
mapWithTag: true
icon: check
tagNames:
filesPaths:
bookmarksGroups:
excludes:
extends:
savedViews: []
favoriteView:
fieldsOrder: []
fields:
- name: realizes
  type: MultiFile
  options:
    dvQueryString: "dv.pages('#operation/Objective and !\"metadata/templates\"')"
  path: ""
  id: f1571278562
- name: involves
  type: MultiFile
  options:
    dvQueryString: "dv.pages('#operation/Entity or #operation/Actor and !\"metadata/templates\"')"
  path: ""
  id: f1558460059
- name: isImplementedBy
  type: MultiFile
  options:
    dvQueryString: "dv.pages('#function/Exchange and !\"metadata/templates\"')"
  path: ""
  id: f110296358
- name: isSupportedBy
  type: File
  options:
    dvQueryString: "dv.pages('#component/System and !\"metadata/templates\"')"
  path: ""
  id: f1082886058
- name: specializes
  type: MultiFile
  options:
    dvQueryString: "dv.pages('#operation/Capability and !\"metadata/templates\"')"
  path: ""
  id: f807053698
- name: isSpecializedBy
  type: MultiFile
  options:
    dvQueryString: "dv.pages('#operation/Capability and !\"metadata/templates\"')"
  path: ""
  id: f1607020784
- name: contains
  type: MultiFile
  options:
    dvQueryString: "dv.pages('#operation/Capability and !\"metadata/templates\"')"
  path: ""
  id: f899675353
- name: isContainedBy
  type: File
  options:
    dvQueryString: "dv.pages('#operation/Capability and !\"metadata/templates\"')"
  path: ""
  id: f2049090498
- name: hasDescription
  type: Input
  path: ""
  id: f1940749968
---