# 连接设备
连接指定的手机，实现手机自动化。
## 属性
### 安卓
 - **序列号**：连接安卓手机设备的序列号，当**平台类型**选择**Andriod**时，出现此属性。

### iOS
- **UUID**： 连接iOS手机设备的UUID，支持一键填充。
- **版本号**：连接iOS手机设备的版本号，支持一键填充。
- **设备名称**：连接iOS手机设备的设备名称，支持一键填充。

### 基本
-  **后延迟（毫秒）**：在执行组件操作之后的延迟时间（以毫秒为单位）。
-  **前延迟（毫秒）**：在开始执行组件操作之前的延迟时间（以毫秒为单位）。
-  **失败后继续**：设置当此组件运行失败时，是否忽略此错误继续运行下一个组件。下拉框选择，当选择"是"时，如果该组件运行时遇到错误，该流程也会继续执行下一个组件，并不会停止；当选择"否"时，如果该组件运行时遇到错误，该流程将会停止执行并抛出错误。
-  **显示名称**：默认为该组件的名称。支持更改，用户自定义此组件的显示名称。

### 连接配置

- **平台类型**：连接设备的类型，分为Andriod和iOS。
- **终端地址**：服务端地址，例如："sh.encootech.com:28888 "