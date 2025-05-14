---
linkTitle: RibbonButton
title: Button
type: docs
prev: docs/buttons/
next: docs/buttons/switchbutton
---

## 1 Overview
+ Parent：Button
+ Demonstrate:
<div align="center">
    <div align="center">
        <img src=" /imgs/RibbonButton/RB-light.png" alt="RibbonButton Light Style" style="width:30%; height:auto;">
        <img src=" /imgs/RibbonButton/RB-dark.png" alt="RibbonButton Dark Style" style="width:30%; height:auto;">
    </div>
    <p align="center">RibbonButton Light/Dark Style</p>
</div>

## 2 Properties
### 2.1 `isDarkMode`
- **Type/Description**: `bool`, night mode, default is controlled by `RibbonTheme` property of the same name

### 2.2 `showBg`
- **Type/Description**: `bool`, show button background, default is `True`
- **Demo picture**:  
  ![showBg-pic]( /imgs/RibbonButton/RB-showBg.png)

### 2.3 `showHoveredBg`
- **Type/Description**: `bool`, show mouse overlay background, default is `True`
- **Demo picture**:  
  ![showHoveredBg-pic-1]( /imgs/RibbonButton/RB-showHoveredBg-1.png)  
  ![showHoveredBg-pic-2]( /imgs/RibbonButton/RB-showHoveredBg-2.png)

### 2.4 `adaptHeight`
- **Type/Description**: `bool`, adapt the height of the button to the parent container, default is `False`
- **Demo picture**:  
  ![adaptHeight-pic]( /imgs/RibbonButton/RB-adaptHeight.png)

### 2.5 `showTooltip`
- **Type/Description**: `bool`, show `Tooltip` floating window, default is `True`
- **Demo picture**:  
  ![showTooltip-pic]( /imgs/RibbonButton/RB-showTooltip.png)

### 2.6 `iconSource`
- **Type/Description**: `var`, button icon, support input image link (`qrc://` or `file://`) or use embedded Microsoft icons (`RibbonIcons`)
- **Demo picture**:  
  ![iconSource-pic]( /imgs/RibbonButton/RB-iconSource.png)

### 2.7 `iconSourceFilled`
- **Type/Description**: `var`，since the code for the hollow and solid versions of Microsoft icons are not fully matched, if the solid icon is abnormal when using inline Microsoft icons and only using iconSource, please replace `RibbonIcons` with `RibbonIcons_Filled` , just like `RibbonIcons.Home -> RibbonIcons_Filled.Home`, and assign the value to this attribute

### 2.8 `imageIcon`
- **Type/Description**: `alias`, direct access to button's image icon object

### 2.9 `ribbonIcon`
- **Type/Description**: `alias`, direct access to button's embedded icon object

### 2.10 `bgColor`
- **Type/Description**: `string`，defines the background color of the button, by default it will switch with the light/dark theme

### 2.11 `hoverColor`
- **Type/Description**: `string`，defines the color when the mouse over the button, default will switch with light/dark theme and whether to show the button background or not

### 2.12 `pressedColor`
- **Type/Description**: `string`，define the color of the button pressed, default will switch with light/dark theme and whether to show button background or not

### 2.13 `checkedColor`
- **Type/Description**: `string`，define the color of the button when it is checked, default is same as `pressedColor`

### 2.14 `textColor`
- **Type/Description**: `string`，define the color of the button text, default is black for light theme and white for dark theme

### 2.15 `textColorReverse`
- **Type/Description**: `bool`，text color rendering, default is `True`, when the button has no background, if the button is covered/pressed/selected by the mouse, the text color of the button will be lightened to render it as a highlight (only noticeable when dark color is used, this attribute has the possibility to be cancelled)

## 3 Example Code
### 3.1 Basic Button
#### 3.1.1 Code
```qml
RibbonButton{
    text:"Button"
}

RibbonButton{
    text:"Button"
    showTooltip: false // don't show the button tip floater
}
```
#### 3.1.2 Code Preview
<div align="center">
    <div align="center">
        <img src=" /imgs/RibbonButton/RB-basicBtn.png" alt="RibbonButton Light Style" style="width:20%; height:auto;">
    </div>
    <p align="center">Basic button</p>
</div>

### 3.2 Basic Button With Icon
#### 3.2.1 Code
```qml
RibbonButton{
    text:"Button"
    iconSource: RibbonIcons.Accessibility
}

RibbonButton{
    text:"Button"
    showBg:false // don't show background
    iconSource: RibbonIcons.Beaker
    checkable: true // let it could be checked
}
```
#### 3.2.2 Code Preview
<div align="center">
    <div align="center">
        <img src=" /imgs/RibbonButton/RB-basicBtnWithIcon.png" alt="RibbonButton Light Style" style="width:30%; height:auto;">
    </div>
    <p align="center">Basic button with icon</p>
</div>

### 3.3 Icon Button
#### 3.3.1 Code
```qml
RibbonButton{
    showBg:false // don't show background
    iconSource: RibbonIcons.Badge
    iconSourceFilled: RibbonIcons_Filled.Badge // define solid icon
    checkable: true // let it could be checked
    tipText: "Button" // define the button tip floater's text
}
RibbonButton{
    showBg:false
    iconSource: RibbonIcons.Clock
    iconSourceFilled: RibbonIcons_Filled.Clock
    tipText: "Button"
}
RibbonButton{
    showBg:false
    iconSource: RibbonIcons.Board
    iconSourceFilled: RibbonIcons_Filled.Board
    checkable: true
    tipText: "Button"
    showTooltip: false // don't show the button tip floater
}
```
#### 3.3.2 Code Preview
<div align="center">
    <div align="center">
        <img src=" /imgs/RibbonButton/RB-iconBtn.png" alt="RibbonButton Light Style" style="width:5%; height:auto;">
    </div>
    <p align="center">Icon button</p>
</div>
