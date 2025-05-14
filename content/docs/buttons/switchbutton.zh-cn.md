---
linkTitle: RibbonSwitchButton
title: 开关按钮
type: docs
prev: docs/buttons/button
next: docs/buttons/pushbutton
---

## 1 概述
+ 父类：Button
+ 展示：
<div align="center">
    <div align="center">
        <img src=" /imgs/RibbonSwitchButton/RSB-light.png" alt="RibbonSwitchButton Light Style" style="width:30%; height:auto;">
        <img src=" /imgs/RibbonSwitchButton/RSB-dark.png" alt="RibbonSwitchButton Dark Style" style="width:30%; height:auto;">
    </div>
    <p align="center">RibbonSwitchButton Light/Dark Style</p>
</div>

## 2 属性
以下是根据您的要求格式化后的表格内容，每项从2.1开始编号，并依次递增：

### 2.1 `isDarkMode`
- 类型: `bool`
- 描述: 夜间模式，默认由`RibbonTheme`的同名属性控制。

### 2.2 `showGrabberText`
- 类型: `bool`
- 描述: 显示抓握指示器的文本，默认文本为`Open`/`Close`。
- 示例图片: ![]( /imgs/RibbonSwitchButton/RSB-showGrabberText.png)

### 2.3 `grabberText`
- 类型: `string`
- 描述: 默认为开关被选中（checked）时为`Open`，否则为`Close`。

### 2.4 `textColor`
- 类型: `string`
- 描述: 开关的标签文本颜色，默认夜间模式为`white`，反之为`black`。
- 示例图片: ![]( /imgs/RibbonSwitchButton/RSB-textColor.png)

### 2.5 `textSize`
- 类型: `int`
- 描述: 开关的标签文本大小。

### 2.6 `grabberCheckedColor`
- 类型: `string`
- 描述: 开关被选中情况下抓握指示器的背景颜色，默认夜间模式下为`#8AAAEB`，反之为`#2850A4`。
- 示例图片: ![]( /imgs/RibbonSwitchButton/RSB-grabberCheckedColor.png)

### 2.7 `grabberUncheckedColor`
- 类型: `string`
- 描述: 开关未被选中情况下抓握指示器的背景颜色，默认夜间模式下为`#292929`，反之为`white`。
- 示例图片: ![]( /imgs/RibbonSwitchButton/RSB-grabberUncheckedColor.png)

### 2.8 `grabberTextCheckedColor`
- 类型: `string`
- 描述: 开关被选中情况下抓握指示器的文本颜色，默认夜间模式下为`black`，反之为`white`。
- 示例图片: ![]( /imgs/RibbonSwitchButton/RSB-grabberTextCheckedColor.png)

### 2.9 `grabberTextUncheckedColor`
- 类型: `string`
- 描述: 开关未被选中情况下抓握指示器的文本颜色，默认夜间模式下为`white`，反之为`black`。
- 示例图片: ![]( /imgs/RibbonSwitchButton/RSB-grabberTextUncheckedColor.png)

### 2.10 `grabberColor`
- 类型: `string`
- 描述: 抓握指示器颜色。
- 示例图片: ![]( /imgs/RibbonSwitchButton/RSB-grabberColor.png)

### 2.11 `borderColor`
- 类型: `string`
- 描述: 开关的边框颜色，默认夜间模式下为`white`，反之为`#616161`。
- 示例图片: ![]( /imgs/RibbonSwitchButton/RSB-borderColor.png)

### 2.12 `borderWidth`
- 类型: `real`
- 描述: 开关的边框宽度，默认为`1.4`。
- 示例图片: ![]( /imgs/RibbonSwitchButton/RSB-borderColor.png) [注：示例图片与`borderColor`共享]

### 2.13 `textBold`
- 类型: `bool`
- 描述: 开关标签文本粗体显示，默认为`false`。

### 2.14 `textOnLeft`
- 类型: `bool`
- 描述: 开关标签文本显示在开关左边，默认为`false`。
- 示例图片: ![]( /imgs/RibbonSwitchButton/RSB-textOnLeft.png)

### 2.15 `showTooltip`
- 类型: `bool`
- 描述: 显示按钮提示浮窗，默认为`False`。

### 2.16 `tipText`
- 类型: `string`
- 描述: 按钮提示文本。

## 3 示例代码
### 3.1 显示抓握指示器文本的开关
#### 3.1.1 代码
```qml
RibbonSwitchButton{
    text: "Button"
    showGrabberText: true // 显示抓握指示器的文本
    textOnLeft: false // 让开关标签显示在开关左边
    grabberCheckedColor: "indigo" // 抓握指示器颜色
}
```

#### 3.1.2 代码预览
<div align="center">
    <div align="center">
        <img src=" /imgs/RibbonSwitchButton/RSB-switchWithGrabberText.png" alt="RibbonSwitchButton With Grabber Text" style="width:20%; height:auto;">
    </div>
    <p align="center">RibbonSwitchButton With Grabber Text</p>
</div>

### 3.2 不显示抓握指示器文本的开关
#### 3.2.1 代码
```qml
RibbonSwitchButton{
    text: "Button"
    showGrabberText: false // 显示抓握指示器的文本
    textOnLeft: false // 让开关标签显示在开关左边
    grabberCheckedColor: "indigo" // 抓握指示器颜色
}
```

#### 3.2.2 代码预览
<div align="center">
    <div align="center">
        <img src=" /imgs/RibbonSwitchButton/RSB-switchWithoutGrabberText.png" alt="RibbonSwitchButton With Grabber Text" style="width:20%; height:auto;">
    </div>
    <p align="center">RibbonSwitchButton Without Grabber Text</p>
</div>