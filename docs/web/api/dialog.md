---
title: Dialog 对话框
description: 对话框是一种临时窗口，通常在不想中断整体任务流程，但又需要为用户展示信息或获得用户响应时，在页面中打开一个对话框承载相应的信息及操作。
isComponent: true
usage: { title: 'Live Demo', description: '' }
spline: message
---

### 确认类对话框

指带有取消及主要操作，指导用户进行二次确认的对话框。常用于反馈或容错的场景。

{{ base }}

### 反馈类对话框

指显示某操作结果的对话框，标题区域有图标，仅有一个确认按钮。常用于操作后结果的展示，或危险、警告等信息的展示。

{{ warning }}

### 异步加载类对话框

按钮带加载标识，操作需要异步完成的对话框。适用于当前操作需要异步完成，等待后再自动关闭对话框。

{{ async }}

### 自定义类对话框

可自定义对话框内容和底部按钮。

{{ custom }}

### 模态与非模态类对话框

模态对话框会中断用户操作，必须处理当前对话框内容后才能进行其他操作。非模态框不中断用户操作。

{{ modal }}

### 弹出位置
可以通过 `placement` 和 `top` 属性来自定义控制对话框位置。

{{ position }}


### 挂载元素

指定对话框元素挂载 DOM。

{{ attach }}

### 插件函数式调用
插件调用方式一：`this.$dialog(options)`

插件调用方式二：`this.$dialog.confirm(options)`

插件调用方式三：`this.$dialog.alert(options)`

<br />

函数调用方式一：`DialogPlugin(options)`

函数调用方式二：`DialogPlugin.confirm(options)`

函数调用方式三：`DialogPlugin.alert(options)`

<br />

组件实例：`DialogInstance = this.$dialog(options)` 或者 组件实例：`DialogInstance = DialogPlugin(options)`

组件实例方法-销毁弹框：`DialogInstance.destroy()`

组件实例方法-隐藏弹框：`DialogInstance.hide()`

组件实例方法-显示弹窗：`DialogInstance.show()`

组件实例方法-更新弹框：`DialogInstance.update()`

{{ plugin }}
