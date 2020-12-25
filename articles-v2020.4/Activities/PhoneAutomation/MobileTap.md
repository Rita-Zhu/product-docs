# 点击
模拟人工进行点击手机屏幕的指定位置。
## 属性
### 点击
- **点击类型**：选择模拟点击的类型，通过下拉框选择。有4种类型：单击，双击，按下，松开。
- **光标位置**：描述从 **横坐标偏移** 和 **纵坐标偏移** 属性添加偏移量的光标的起点。默认选项是**中心**。
- **横坐标百分比**：根据**光标位置**进行百分比移动。以点击所指定矩形框的长度为基数，乘以此属性值，结果和 **光标位置**的横坐标相加，得到最终的点击横坐标。

    例如填写"0.5",光标位置选择"中心"，最终点击位置的计算过程：取指定元素的矩形框长度，乘以0.5，结果为矩形框长度的一半；后和光标位置"中心"执行相加计算，最终得到的数字为点击的横坐标，即为矩形框的右边框中心处。
    
- **横坐标偏移**：根据**光标位置**字段中选择的选项，光标位置的水平位移像素量。例如填写“10”，则代表以**光标位置**为开始，向右偏移10个像素。计算坐标时，以屏幕左上角为原点。仅支持整型变量和整型。
- **纵坐标百分比**：根据**光标位置**进行百分比移动。以点击所指定矩形框的宽度为基数，乘以此属性值，结果和 **光标位置**的纵坐标相加，得到最终的点击纵坐标。

    例如填写"0.5",光标位置选择"中心"，最终点击位置的计算过程：取指定元素的矩形框宽度，乘以0.5，结果为矩形框宽度的一半；后和光标位置"中心"执行相加计算，最终得到的数字为点击的纵坐标，即为矩形框的下边框中心处。
- **纵坐标偏移**：根据**光标位置**字段中选择的选项，光标位置的垂直位移像素量。例如填写“10”，则代表以**光标位置**为开始，向下偏移10个像素。计算坐标时，以屏幕左上角为原点。仅支持整型变量和整型。


### 基本
-  **超时（毫秒）**：指定最长等待时间（以毫秒为单位），如果超出该时间后组件未执行，系统会抛出错误。
-  **后延迟（毫秒）**：在执行组件操作之后的延迟时间（以毫秒为单位）。
-  **前延迟（毫秒）**：在开始执行组件操作之前的延迟时间（以毫秒为单位）。
-  **失败后继续**：设置当此组件运行失败时，是否忽略此错误继续运行下一个组件。下拉框选择，当选择"是"时，如果该组件运行时遇到错误，该流程也会继续执行下一个组件，并不会停止；当选择"否"时，如果该组件运行时遇到错误，该流程将会停止执行并抛出错误。
-  **显示名称**：默认为该组件的名称。支持更改，用户自定义此组件的显示名称。

### 可选项
- **彩色识别**：仅当图像识别时，才出现此属性，默认为否。
- **阈值**：仅当图像识别时，和出现此属性，默认为0.75，值越大，匹配越严格。

### 目标
- **[选择器](../Appendix/Selector.md?_v=v2020.4)**：用于指示要点击的目标位置。可通过点击**指定元素**自动生成。仅支持字符串变量和字符串。