# 日期和时间选择框

流程运行时弹窗让用户选择日期和时间并输出。
>**说明：**
>
>运行时窗口中默认显示为当前日期和时间。

## 属性

### 基本

- **显示名称** ：默认为该组件的名称。支持更改，用户自定义此组件的显示名称
- **失败后继续** ：设置当此组件运行失败时，是否忽略此错误继续运行下一个组件。下拉框选择，当选择"是"时，如果该组件运行时遇到错误，该流程也会继续执行下一个组件，并不会停止；当选择"否"时，如果该组件运行时遇到错误，该流程将会停止执行并抛出错误
- **前延时(毫秒)** ：指定在此组件执行前的等待时间。单位为毫秒（ms）,1000ms = 1s。若此处填写1000，意为上一个组件执行完毕后，等待一秒钟后执行此组件
- **后延时(毫秒)** ：指定在此组件执行后的延迟时间。单位为毫秒（ms）,1000ms = 1s。若此处填写1000，意为此组件执行完毕后，等待一秒钟后执行下一个组件


### 输出

- **选择的时间** ：输出用户在弹窗中指定的日期和时间，仅可接变量。
  
### 输入

- **标题**：（非必填）自定义**日期和时间选择框**组件运行时的标题，可接变量。
- **描述**：（非必填）自定义**日期和时间选择框**组件运行时的描述信息，可接变量。

## 操作样例
1. 拖入**日期和时间选择框**组件到设计面板：
![](https://docimages.blob.core.chinacloudapi.cn/images/Activities/timePicker-1.png)

2. 双击进入组件内部，配置属性参数。

   ![](https://docimages.blob.core.chinacloudapi.cn/images/Activities/timePicker-2.png)

- 标题：自定义日期和时间选择框组件运行时的标题，如，“时间”；
- 描述：自定义日期和时间选择框组件运行时的描述信息，如，“当前时间为：”；
- 输出：输出用户在弹窗中指定的日期和时间，如，这里我们指定当前时间：

3. 拖入**写入日志**组件：
![](https://docimages.blob.core.chinacloudapi.cn/images/Activities/timePicker-3.png)

4. 运行流程，弹窗让用户选择日期和时间并输出：
![](https://docimages.blob.core.chinacloudapi.cn/images/Activities/timePicker-4.png)
![](https://docimages.blob.core.chinacloudapi.cn/images/Activities/timePicker-5.png)
