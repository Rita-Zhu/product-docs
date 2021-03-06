# 确认框

以弹框形式将需要人工确认的信息展现出来，并可通过用户的确认结果（确认，取消）来做后续判断与流程走向的控制

## 属性

### 基本

- **显示名称** ：默认为该组件的名称。支持更改，用户自定义此组件的显示名称
- **失败后继续** ：设置当此组件运行失败时，是否忽略此错误继续运行下一个组件。下拉框选择，当选择"是"时，如果该组件运行时遇到错误，该流程也会继续执行下一个组件，并不会停止；当选择"否"时，如果该组件运行时遇到错误，该流程将会停止执行并抛出错误
- **前延时(毫秒)** ：指定在此组件执行前的等待时间。单位为毫秒（ms）,1000ms = 1s。若此处填写1000，意为上一个组件执行完毕后，等待一秒钟后执行此组件
- **后延时(毫秒)** ：指定在此组件执行后的延迟时间。单位为毫秒（ms）,1000ms = 1s。若此处填写1000，意为此组件执行完毕后，等待一秒钟后执行下一个组件


### 输入

- **标题** ：弹出的确认框的标题。仅支持字符串变量和字符串
- **描述** ：弹出的确认框中，需要确认的描述信息。仅支持字符串变量和字符串

### 输出

- **确认结果** ：将确认结果的值存储在此变量。点击&quot;确认&quot;按钮后的返回值为True; 点击&quot;取消&quot;按钮后的返回值为False
  
## 操作样例

1. 拖入一个**确认框**组件至流程中。
2. 双击**确认框**组件的空白处，配置属性参数。
   ![确认框配置](https://docimages.blob.core.chinacloudapi.cn/images/Activities/comfirmsetting20201221.png)  

    - 标题：输入确认框的标题，如，"确认"
    - 描述：输入确认框的描述内容，如，"请确认，是否弹框？"
3. 保存并运行流程。
4. 查看运行结果，如下图所示。

   ![查看运行结果](https://docimages.blob.core.chinacloudapi.cn/images/Activities/showresult20201221.png)
