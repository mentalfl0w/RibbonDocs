---
linkTitle: RibbonSwitchButton
title: Switch Button
type: docs
prev: docs/buttons/button
next: docs/buttons/pushbutton
---

## 1 Overview
+ Parent class: Button
+ Demonstrate:
<div align="center">
    <div align="center">
        <img src="/imgs/RibbonSwitchButton/RSB-light.png" alt="RibbonSwitchButton Light Style" style="width:30%; height:auto;">
        <img src="/imgs/RibbonSwitchButton/RSB-dark.png" alt="RibbonSwitchButton Dark Style" style="width:30%; height:auto;">
    </div>
    <p align="center">RibbonSwitchButton Light/Dark Style</p>
</div>

## 2 Properties
### 2.1 `isDarkMode`
- Description: `bool`, Night mode, controlled by the same-named property of `RibbonTheme` by default.

### 2.2 `showGrabberText`
- Description: `bool`, Display the text of the grabber indicator, default text is `Open`/`Close`.
- Example Image: ![showGrabberText-pic](/imgs/RibbonSwitchButton/RSB-showGrabberText.png)

### 2.3 `grabberText`
- Description: `string`, Default is `Open` when the switch is checked, otherwise `Close`.

### 2.4 `textColor`
- Description: `string`, The color of the switch's label text, default is `white` in night mode, otherwise `black`.
- Example Image: ![textColor-pic](/imgs/RibbonSwitchButton/RSB-textColor.png)

### 2.5 `textSize`
- Description: `int`, The size of the switch's label text.

### 2.6 `grabberCheckedColor`
- Description: `string`, The background color of the grabber indicator when the switch is checked, default is `#8AAAEB` in night mode, otherwise `#2850A4`.
- Example Image: ![grabberCheckedColor-pic](/imgs/RibbonSwitchButton/RSB-grabberCheckedColor.png)

### 2.7 `grabberUncheckedColor`
- Description: `string`, The background color of the grabber indicator when the switch is not checked, default is `#292929` in night mode, otherwise `white`.
- Example Image: ![grabberUncheckedColor-pic](/imgs/RibbonSwitchButton/RSB-grabberUncheckedColor.png)

### 2.8 `grabberTextCheckedColor`
- Description: `string`, The text color of the grabber indicator when the switch is checked, default is `black` in night mode, otherwise `white`.
- Example Image: ![grabberTextCheckedColor-pic](/imgs/RibbonSwitchButton/RSB-grabberTextCheckedColor.png)

### 2.9 `grabberTextUncheckedColor`
- Description: `string`, The text color of the grabber indicator when the switch is not checked, default is `white` in night mode, otherwise `black`.
- Example Image: ![grabberTextUncheckedColor-pic](/imgs/RibbonSwitchButton/RSB-grabberTextUncheckedColor.png)

### 2.10 `grabberColor`
- Description: `string`, The color of the grabber indicator.
- Example Image: ![grabberColor-pic](/imgs/RibbonSwitchButton/RSB-grabberColor.png)

### 2.11 `borderColor`
- Description: `string`, The border color of the switch, default is `white` in night mode, otherwise `#616161`.
- Example Image: ![borderColor-pic](/imgs/RibbonSwitchButton/RSB-borderColor.png)

### 2.12 `borderWidth`
- Description: `real`, The width of the switch's border, default is `1.4`.
- Example Image: ![borderColor-pic](/imgs/RibbonSwitchButton/RSB-borderColor.png)

### 2.13 `textBold`
- Description: `bool`, Display the switch label text in bold, default is `false`.

### 2.14 `textOnLeft`
- Description: `bool`, Display the switch label text on the left side of the switch, default is `false`.
- Example Image: ![textOnLeft-pic](/imgs/RibbonSwitchButton/RSB-textOnLeft.png)

### 2.15 `showTooltip`
- Description: `bool`, Display button tooltip, default is `false`.

### 2.16 `tipText`
- Description: `string`, Button tooltip text.

## 3 Example Code
### 3.1 Switch with Grabber Indicator Text
#### 3.1.1 Code
```qml
RibbonSwitchButton{
    text: "Button"
    showGrabberText: true // Display the text of the grabber indicator
    textOnLeft: false // Let the switch label display on the left side of the switch
    grabberCheckedColor: "indigo" // The color of the grabber indicator
}
```

#### 3.1.2 Code Preview
<div align="center">
    <div align="center">
        <img src="/imgs/RibbonSwitchButton/RSB-switchWithGrabberText.png" alt="RibbonSwitchButton With Grabber Text" style="width:20%; height:auto;">
    </div>
    <p align="center">RibbonSwitchButton With Grabber Text</p>
</div>

### 3.2 Switch without Grabber Indicator Text
#### 3.2.1 Code
```qml
RibbonSwitchButton{
    text: "Button"
    showGrabberText: false // Do not display the text of the grabber indicator
    textOnLeft: false // Let the switch label display on the left side of the switch
    grabberCheckedColor: "indigo" // The color of the grabber indicator
}
```

#### 3.2.2 Code Preview
<div align="center">
    <div align="center">
        <img src="/imgs/RibbonSwitchButton/RSB-switchWithoutGrabberText.png" alt="RibbonSwitchButton With Grabber Text" style="width:20%; height:auto;">
    </div>
    <p align="center">RibbonSwitchButton Without Grabber Text</p>
</div>