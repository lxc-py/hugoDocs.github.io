---
title: '作业界面'
linkTitle: '作业界面'
weight: 4
---

在作业页面中，用户(例如，具有工作人员角色的用户)可以查看分配给他们的作业，而无需访问任务页面，

以及跟踪进度，排序和应用过滤器到工作列表.

![](/images/image243_detrac.jpg)

在作业页面上，有表格显示作业列表.
每一行数据包括:
- 作业ID
- 项目名
- 任务名
- 已标注图像数量
- [阶段][stage] and [状态][state]
- 合格率
- 不良张数
- 工作人员.

> 要在新选项卡中打开该作业,按住`Ctrl`单击该作业ID.

在左上角有一个搜索栏，你可以使用它来查找被分配人员、阶段、状态等。

右上角有[排序][sorting]， [快速筛选][quick-filters]和筛选.

## 筛选

> 应用筛选器禁用[快速筛选器][quick-filters].

筛选器的工作原理与标注过滤器类似，
你可以从[属性](#支持为作业列表的属性)中创建规则 [运算符][operators]
和值 并将规则 [分组][groups]. 有关详细信息,请参阅 [筛选部分][create-filter].
了解更多关于[日期和时间选择][data-and-time].

要清除所有筛选,请单击 `清除筛选`.

### 支持为作业列表的属性

| 属性     | 支持的值                             | 描述                                 |
| -------------- | -------------------------------------------- | ------------------------------------------- |
| `状态`        | 所有状态的名称                       | 作业状态<br>(可在作业内的菜单中更改) |
| `阶段`        | 所有阶段的名称                       | 作业的阶段<br>(通过任务页面上的下拉列表指定) |
| `维度`    | `2D` 或 `3D`                                 | 取决于数据格式 |
| `分配`     | 用户名                                     | 分配人员是正在工作的用户。<br>(在任务页上指定) |
| `上次更新` | 最后修改的日期和时间(或取值范围)|日期可以以' dd.MM.yyyy HH:mm '格式输入，也可以在单击输入框时出现的窗口中选择日期 |
| `ID`           | 作业ID的数字或范围                   |                                             |
| `任务ID`      | 任务ID的数字或范围                   |                                             |
| `项目ID`   | 项目ID的数字或范围                |                                             |
| `任务名称`    | 任务名称                                    | 在创建任务时设置，<br>可以在([任务页面](/docs/manual/basics/task-details/)) 中更改|
| `项目名称` | 项目名称                                | 在创建项目时指定，<br>可以在([项目部分](/docs/manual/advanced/projects/))上进行更改 |

[state]: /docs/manual/basics/vocabulary/#状态
[stage]: /docs/manual/basics/vocabulary/#阶段
[create-task]: /docs/manual/basics/creating_an_annotation_task
[create-filter]: /docs/manual/advanced/filter/#新建筛选
[operators]: /docs/manual/advanced/filter/#支持的属性运算符
[groups]: /docs/manual/advanced/filter/#分组
[data-and-time]: /docs/manual/advanced/filter#日期和时间的选择
[sorting]: /docs/manual/advanced/filter/#排序
[quick-filters]: /docs/manual/advanced/filter/#快速筛选
