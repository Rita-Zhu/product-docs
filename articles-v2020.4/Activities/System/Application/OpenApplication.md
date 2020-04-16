# 打开程序

用于启动指定的应用程序并在其中执行多个组件。
对于要打开的目标应用程序，有两种定位方法：
1. 自动生成：使用**指定程序**功能，自动生成**选择器**和**文件名称**属性，无需用户手动填写属性值
2. 手动填写：不适用**指定程序**功能,手动填写目标程序的安装路径

## 属性
基本
- **显示名称** ：默认为该组件的名称。支持更改，用户自定义此组件的显示名称
- **失败后继续** ：设置当此组件运行失败时，是否忽略此错误继续运行下一个组件。下拉框选择，当选择"是"时，如果该组件运行时遇到错误，该流程也会继续执行下一个组件，并不会停止；当选择"否"时，如果该组件运行时遇到错误，该流程将会停止执行并抛出错误
- **前延时(毫秒)** ：指定在此组件执行前的等待时间。单位为毫秒（ms）,1000ms = 1s。若此处填写1000，意为上一个组件执行完毕后，等待一秒钟后执行此组件
- **后延时(毫秒)** ：指定在此组件执行后的延迟时间。单位为毫秒（ms）,1000ms = 1s。若此处填写1000，意为此组件执行完毕后，等待一秒钟后执行下一个组件


可选项
- **结束后关闭** ：程序运行结束后是否关闭

目标
- **匹配超时(毫秒)** ：默认为5000毫秒，可配置超时时间

输出
- **程序** ：将目标程序存储在此变量。可作为**关闭程序**的输入值

应用程序
- **参数** ：启动程序时可以传递给应用程序的参数。可以使用此属性使用你要打开的应用程序打开特定的文件.例入要打开特定的Excel工作簿，则可添加其完整路径：**C:\Users\currentuser\Documents\Sample.xlsx**
- **文件名称** ：打开此路径下的可执行文件。可通过点击**指定程序**自动生成，也可以手动填入此属性值。例如要打开Excel,则可填入类似：**C：\Program Files\Microsoft Office\root\Office16\EXCEL.EXE**。仅支持字符串变量和字符串
- **选择器** ：定位指定程序进行打开。可通过点击**指定程序**自动生成。若不使用**指定程序**，手动填写**文件名称**（即此项为空时），则无法实现最大化功能且输出程序变量为空
- **窗口最大化** ：选择是否将打开的程序最大化
- **工作目录** ：目标程序的工作目录。如果在文件名中已给出，则无需填写此项

<table><td bgcolor=	#F0F8FF>使用自动生成属性值<b>指定程序</b>时,请先讲目标程序打开，然后使用<b>指定程序</b>。（指定程序图标和快捷方式无效）</td></table>
