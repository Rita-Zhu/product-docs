# 表格
表格组件用于展示和操作在**数据表管理**中已创建的数据表。
## 添加表格组件
1. 在页面区域单击选中需要添加表格组件的页面。
2. 在组件区域双击或拖拽模块组件中的表格组件至当前选中页面。
3. 在弹出的添加表格组件对话框中，填写相应信息，如下图所示，具体参数说明如下表所示。

![添加表格组件](https://docimages.blob.core.chinacloudapi.cn/images/Kris/AppsV2/addtable20201208.png)

| 参数       | 说明 |
| ---------- | ---- |
| 选择表     |下拉选择该小程序应用中的任一数据表。      |
| 展示列     |可通过下拉列表勾选/反选需要展示的列。      |
| 创建新增页 |勾选后，在运行该组件时，将出现“新增”按钮，点击后可创建新增页。    |
| 创建详情页 |勾选后，在运行该组件时，在“操作”列将出现“详情”链接，点击后创建详情页。    |
| 创建编辑页 |勾选后，在运行该组件时，在“操作”列将出现“编辑”链接，点击后创建编辑页。    |

4. 单击“创建”，根据配置将表格模块组件加载进当前页面并选中该组件。

## 配置表格组件
选中整个表格组件，可在页面右侧对表格组件的参数进行配置，具体参数配置说明如下表所示。

| 参数     | 说明                                                         |
| -------- | ------------------------------------------------------------ |
| 表格名称 | 显示表格组件已关联的数据表名称。                             |
| 布局     | 是否固定列宽，默认不固定，根据列内容长度自适应，单击打开“固定”右侧的开关，则表示根据所设置的列宽进行固定。 |
| 展示列   | 展示选中表的所有列，列名及展示名。<br>支持勾选”隐藏/显示“图标， 显示代表在界面内显示该列，隐藏代表不显示该列。 |
| 表格操作 | 支持对表格的内容进行新增、编辑、删除、查看详情的操作。<br>勾选“隐藏/显示”图标， 显示代表在界面内显示该操作，隐藏代表不显示该操作。其中”删除“按钮不支持关联其它页面，其它按钮支持关联其它需要打开的页面。 |
| 筛选     | 为表格配置一个或多个筛选项，支持按等于、不等于、包含、不包含、为空、不为空对条件列进行筛选。 |
| 排序     | 为表格设置一个或多个排序规则，支持升序和降序排序。           |

## 配置表格列
选中表格组件中的单个表头字段，可在页面右侧对表格字段列的参数进行配置，具体参数配置说明如下表所示。
>**说明:**
>
>支持拖动单个表头字段，对表头字段进行排序。

| 参数                | 说明                                                         |
| ------------------- | ------------------------------------------------------------ |
| 展示名称            | 输入该列需要展示的列名称，默认填写了初始化的列名。           |
| 列宽                | 输入当前列的宽度，单位：px。                                 |
| 控制 - 是否支持筛选 | 是否支持当前列具备筛选功能，默认开关为关闭状态表示不支持。当开关为打开状态时，表头字段右侧出现小漏斗样式的筛选图标，同时支持多列复合筛选。 |
| 控制 - 是否支持排序 | 是否支持当前列具备排序功能，默认开关为关闭状态表示不支持。当开关为打开状态时，表头字段右侧出现上下小箭头样式的排序图标，支持升序和降序排序。 |
| 控制 - 是否固定左侧 | 是否固定最左侧第1列，默认开关为关闭状态表示不固定。当开关为打开状态时，最左侧第1列固定，不随其它列左右滚动而移动。 |