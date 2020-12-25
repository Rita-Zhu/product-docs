# 数组转集合
将数组转换为集合，一般用来遍历数组。

## 属性

### 基本
- **显示名称** ：默认为该组件的名称。支持更改，用户自定义此组件的显示名称
- **失败后继续** ：设置当此组件运行失败时，是否忽略此错误继续运行下一个组件。下拉框选择，当选择"是"时，如果该组件运行时遇到错误，该流程也会继续执行下一个组件，并不会停止；当选择"否"时，如果该组件运行时遇到错误，该流程将会停止执行并抛出错误
- **前延迟(毫秒)** ：指定在此组件执行前的等待时间。单位为毫秒（ms）,1000ms = 1s。若此处填写1000，意为上一个组件执行完毕后，等待一秒钟后执行此组件
- **后延迟(毫秒)** ：指定在此组件执行后的延迟时间。单位为毫秒（ms）,1000ms = 1s。若此处填写1000，意为此组件执行完毕后，等待一秒钟后执行下一个组件
### 输入

- **数组**：欲被转换为集合的数组，可接变量。

### 输出

- **集合**：被转换成的集合对象的结果，仅可接变量。

## 操作样例
1. 拖入一个**数组转集合**组件至流程中。
2. 定义两个流程变量：
   ![定义变量](https://docimages.blob.core.chinacloudapi.cn/images/Activities/varials20201218.png)
   - CL：此变量用于存放转换后的集合的值，变量类型定义为`List<Int32>`
   - array：此变量用于存放待转成集合的数组，变量类型定义为`Int32[]`，并输入默认值为`new int[]{1,3,5,7,9};`  

3. 配置**数组转集合**组件的属性。
   ![赋值](https://docimages.blob.core.chinacloudapi.cn/images/Activities/assign20201218.png)

   - 集合：将定义的CL变量赋值给集合，输入`CL`
   - 数组：将定义的array变量赋值给数组，输入`array`  

4. 在**数组转集合**组件的下方拖入一个**写入日志**组件，并双击配置该组件，输入`"数组转集合的值为"+CL.First()`，表示获取集合中的第一个值。

5. 保存并运行流程。
6. 在输出窗口查看运行结果。
   ![查看运行结果](https://docimages.blob.core.chinacloudapi.cn/images/Activities/arraytolistresult20201218.png)