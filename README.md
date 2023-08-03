# bpmn-js-properties-panel-for-activiti
A library based on BPMN-Js-Property-panel modified to support the activiti engine.

一个基于bpmn-js-properties-panel进行改造成支持activiti引擎的库。

## 如何使用呢？

### 1、npm安装依赖

```shell
npm install bpmn-js-properties-panel-for-activiti
```

### 2、引入模块

```js
import "bpmn-js-properties-panel-for-activiti/dist/assets/bpmn-js-properties-panel-for-activiti.css"
import propertiesPanelModule from "bpmn-js-properties-panel-for-activiti"
import propertiesProviderModule from "bpmn-js-properties-panel-for-activiti/lib/provider/activiti"
import activitiModdleExtension from "bpmn-js-properties-panel-for-activiti/config/activiti.json"
```

### 3、添加即可

```js
  new BpmnModeler({
    container: document.getElementById("canvas"),
    propertiesPanel: {
      parent: "#properties"
    },
    additionalModules: [
      propertiesPanelModule,
      propertiesProviderModule,
    ],
    moddleExtensions: {
      activiti: activitiModdleExtension
    }
  })
```
