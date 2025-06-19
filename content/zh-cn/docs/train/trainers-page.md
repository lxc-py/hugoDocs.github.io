---
title: '训练任务页面'
linkTitle: '训练任务页面'
weight: 6
description: '训练任务页面概览.'
---

![](/images/trainers_page.png)

任务页面包含元素，每个元素与一个单独的任务相关。它们按创建顺序排序.
每个元素包含:任务名称，进度条，按钮 `打开`, 菜单 `动作`.
每个按钮负责菜单中的`动作`特定功能:

- `导出模型` — 下载该训练训练出的特定格式的模型文件.
- `验证模型` - 使用该模型文件创建推理任务
- `删除` — 删除训练任务.

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
| `状态`       |  `已完成`或`未完成`    |                                             |
| `模型`       | 模型类型                      |
| `油墨`     | AVI所添加的油墨                                  | |
| `开始时间`        | 开始训练的时间                                     | 日期可以以' dd.MM.yyyy HH:mm '格式输入，也可以在单击输入框时出现的窗口中选择日期 |
| `完成时间` | 完成训练的时间|日期可以以' dd.MM.yyyy HH:mm '格式输入，也可以在单击输入框时出现的窗口中选择日期 |
| `名称`         | 名称                                         | |

---

按`打开`按钮进入[任务详情](/docs/train/train-details/).


[create-filter]: /docs/manual/advanced/filter/#新建筛选
[operators]: /docs/manual/advanced/filter/#支持的属性运算符
[groups]: /docs/manual/advanced/filter/#分组
[data-and-time]: /docs/manual/advanced/filter#日期和时间的选择
[sorting]: /docs/manual/advanced/filter/#排序
[quick-filters]: /docs/manual/advanced/filter/#快速筛选