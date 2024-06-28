---
title: '任务页面'
linkTitle: '任务页面'
weight: 5
description: '任务页面概览.'
---

![](/images/image006_detrac.jpg)

任务页面包含元素，每个元素与一个单独的任务相关。它们按创建顺序排序.
每个元素包含:任务名称，预览，进度条，按钮 `打开`, 菜单 `动作`.
每个按钮负责菜单中的`动作`特定功能:

- `导出任务数据集` — 下载特定格式的标注或标注和图像.
  更多信息请参阅[导出/导入数据集](/docs/manual/advanced/export-import-datasets/)
  部分.
- `上传标注` 以特定格式上传标注.
   更多信息请参阅[导出/导入数据集](/docs/manual/advanced/export-import-datasets/)
  部分.
- `自动标注` — 未开发.
- `备份任务` — 将此任务备份到zip归档文件中.
  更多信息请参阅[备份](/docs/manual/advanced/backup/)部分.
- `移动到项目` — 将任务移动到项目(只能移动不属于任何项目的任务)。
如果标签不匹配，您可以在项目/任务中创建或删除必要的标签。
有些任务标签可以与目标项目标签相匹配.
- `删除` — 删除任务.

在左上角有一个搜索栏，使用它你可以找到任务的分配人员，任务名称等.
右上角有[排序][sorting], [快速筛选][quick-filters]和筛选.

## 筛选

> 应用筛选器禁用[快速筛选器][quick-filters].

筛选器的工作原理与标注过滤器类似，
你可以从[属性](#支持为任务列表的属性)中创建规则 [运算符][operators]
和值 并将规则 [分组][groups].
有关详细信息,请参阅 [筛选部分][create-filter].
了解更多关于[日期和时间选择][data-and-time].


要清除所有筛选,请单击 `清除筛选`.

### 支持为任务列表的属性

| 属性     | 支持的值                           | 描述                                 |
| -------------- | -------------------------------------------- | ------------------------------------------- |
| `维度`    | `2D` or `3D`                                 | 取决于数据格式 |
| `状态`       | `标注`, `质检` or `已完成`    |                                             |
| `数据`         | `视频`, `图像`                            | 取决于数据格式 |
| `子集`       | `测试`, `训练`, `验证` 或者自定义创建 | [read more] [subset]                      |
| `分配人员`     | 用户名                                     | 分配人员是从事项目、任务或工作的用户。<br>(在任务详情页上指定) |
| `所有者`        | 用户名                                     | 拥有项目、任务或作业的用户 |
| `上次更新` | 最后修改的日期和时间(或取值范围)|日期可以以' dd.MM.yyyy HH:mm '格式输入，也可以在单击输入框时出现的窗口中选择日期 |
| `ID`           | 任务ID的数字或范围                   |                                             |
| `项目ID`   | 项目ID的数字或范围                |                                             |
| `名称`         | 名称                                         | 在“任务”页上-任务的名称，<br>在“项目”页上-项目的名称 |
| `项目名称` | 项目名称                               | 在创建项目时指定，<br>可以在([项目部分](/docs/manual/advanced/projects/))上进行更改|

---

按`打开`按钮进入[任务详情](/docs/manual/basics/task-details/).


[create-filter]: /docs/manual/advanced/filter/#新建筛选
[operators]: /docs/manual/advanced/filter/#支持的属性运算符
[groups]: /docs/manual/advanced/filter/#分组
[data-and-time]: /docs/manual/advanced/filter#日期和时间的选择
[sorting]: /docs/manual/advanced/filter/#排序
[quick-filters]: /docs/manual/advanced/filter/#快速筛选
