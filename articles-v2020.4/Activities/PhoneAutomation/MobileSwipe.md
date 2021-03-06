# 滑动屏幕
模拟人工进行尝手机屏幕效果。
>**说明：**
>
> 该组件仅能放置于**连接设备**组件内，且操作自动绑定至外层设备。

## 属性

### 基本

- **后延迟（毫秒）**：在执行组件操作之后的延迟时间（以毫秒为单位）。
- **前延迟（毫秒）**：在开始执行组件操作之前的延迟时间（以毫秒为单位）。
- **失败后继续**：设置当此组件运行失败时，是否忽略此错误继续运行下一个组件。下拉框选择，当选择"是"时，如果该组件运行时遇到错误，该流程也会继续执行下一个组件，并不会停止；当选择"否"时，如果该组件运行时遇到错误，该流程将会停止执行并抛出错误。
- **显示名称**：默认为该组件的名称。支持更改，用户自定义此组件的显示名称。

### 目标

- **[选择器](../Appendix/Selector.md?_v=v2020.4)**：用于指示要点击的目标位置。可通过点击**指定元素**自动生成。仅支持字符串变量和字符串。

## 操作样例

1. 拖入一个连接设备组件至流程中，具体参见[连接设备组件 - 操作样例](/articles-v2020.4/Activities/PhoneAutomation/MobileConnect.md)。
2. 在连接设备组件内拖入一个**滑动屏幕**组件。
3. 单击**滑动屏幕**组件中的**指定元素**链接，在移动设备管理器界面按下鼠标左键从左往右或从右往左滑动，如下图所示。
   ![滑动屏幕](https://docimages.blob.core.chinacloudapi.cn/images/Activities/swipescreen20201223.png)

4. 保存并运行流程，可看到屏幕出现左滑或右滑的效果。