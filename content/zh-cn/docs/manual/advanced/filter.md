---
title: '筛选'
linkTitle: '筛选'
weight: 24
description: '使用筛选功能的指南.'
---

使用该功能有一些原因:

1. 使用筛选时，与过滤器不匹配的对象将被隐藏.
2. 快速导航到包含感兴趣对象的帧之间.
   你可以使用键盘上的`左箭头`和`右箭头`键来实现这个目的，
   或者通过右键单击并选择`通过筛选切换`来自定义用户界面按钮。
   如果没有与筛选条件匹配的对象，你将前进到包含任何已注释对象的前一帧或下一帧.

要使用筛选，你需要点击顶部面板上的按钮.

![](/images/image059.jpg)

## 新建筛选

它将打开一个窗口用于筛选输入。在这里你会发现两个按钮:`Add rule`和`Add group`.

![](/images/image202.jpg)

### 规则

`Add rule`按钮为对象显示添加规则。规则可以使用以下属性:

![](/images/image204.jpg)

### 支持的标注属性

| 属性   | 支持的值                                      | 描述                                 |
| ------------ | ------------------------------------------------------ | ------------------------------------------- |
| `标签`      | 任务中的所有标签名称               | 标签名                                  |
| `类型`       | 形状，轨迹或标签                                    | 对象的类型                              |
| `形状`      | 所有形状类型                                        | 形状的类型                               |
| `覆盖`   | 真或假                                          | 覆盖 ([详情](/docs/manual/advanced/shape-mode-advanced/)) |
| `宽度`      | 单位px                                  | 形状宽度                                 |
| `高度`     | 单位px                                   | 形状高度                                |
| `服务器ID`   | 数字                                        | 服务器上对象的ID <br>(您可以通过动作菜单形成到对象的链接来查找) |
| `对象ID`   | 数字                                       | 客户端中对象的ID <br>(在对象侧栏中指出) |
| `属性` | 其他一些字段包括具有<br>类似类型或特定属性值的属性 | 由标签指定的任何字段 |

- [项目列表的支持属性](/docs/manual/advanced/projects/#supported-properties-for-projects-list)

- [任务列表的支持属性](/docs/manual/basics/tasks-page/#supported-properties-for-tasks-list)

- [作业列表的支持属性](/docs/manual/basics/jobs-page/#supported-properties-for-jobs-list)

### 支持的属性运算符

`==` - 等于; `!=` - 不等于; `>` - 大于; `>=` - 大于等于; `<` - 小于; `<=` - 小于等于;

`Any in`; `Not in` - 这些操作符允许您在一条规则中设置多个值;

![](/images/image203.jpg)

`Is empty`; `is not empty` – 这些操作符不需要输入值,意思是为空和非空.

`Between`; `Not between` – 这些操作符允许您在两个值之间选择一个范围.

`Like` - 此操作符指示属性必须包含一个值.

`Starts with`; `Ends with` - 按开头或结尾筛选.

有些属性支持您可以选择的两种类型的值:


您可以添加多个规则，为此单击add rule按钮并设置另一个规则.
一旦你设置了一个新规则，你就可以选择通过哪个操作符来连接它们: `And` 或者 `Or`.

![](/images/image206.jpg)

所有后续规则将由所选的操作符连接.
单击`提交`来应用筛选，或者如果您希望通过不同的操作符连接多个规则，请使用group.

### 分组

要添加组，请单击`Add group`按钮。在组内，您可以创建规则或组.

![](/images/image207.jpg)

如果组中有多个规则，它们可以用`And`或`or`操作符连接.
规则组将像组外的单独规则一样工作，并将由组外的操作员加入.
您可以在其他组中创建组，为此，您需要单击组内的add group按钮.

你可以改变规则和小组。要移动规则或组，请通过按钮拖动它.
要删除规则或组，请单击`删除`按钮.

如果你激活`Not`按钮，不匹配组的对象将被过滤掉.
点击`提交`来应用筛选.
`取消` 按钮取消筛选. `清除筛选`按钮移除筛选.

一旦应用，筛选框自动出现在`最近使用`列表中。列表的最大长度是10.

---

## 排序和筛选列表

在[项目](/docs/manual/advanced/projects/#projects-page), 项目页面上的任务列表,
[任务](/docs/manual/basics/tasks-page/), [作业](/docs/manual/basics/jobs-page/),你可以使用排序和筛选.

> 应用的排序和筛选将显示在您的浏览器的URL,
> 因此，您可以通过应用排序和筛选来共享页面.

### 排序
您可以按以下参数进行排序:
- 作业列表: ID, 分配人, 上次更新, [阶段][stage], [状态][state], 任务ID, p项目ID,
任务名称, 项目名称.
- 任务列表或项目页上的任务列表: ID, 所有者, 状态, 分配人, 上次更新, [子集][subset], [模式][mode],
[维度][dimension], 项目ID, 名称, 项目名称.
- 项目列表: ID, 分配人, 所有者, 状态, 名称, 上次更新.


要应用排序，请将参数拖动到水平栏上方的顶部区域.
水平线以下的参数将不会被应用.
通过移动参数，你可以改变优先级,
首先，排序将根据上述参数进行.

按下`排序按钮`可切换`升序排序`/`降序排序`.

### 快速筛选

快速筛选包含几个常用的筛选:
- `分配给我` - 只显示分配给您的那些项目、任务或工作.
- `归我所有` -  只显示属于您的项目或任务.
- `未完成` - 只显示那些状态不是已完成的项目、任务或作业.

#### 日期和时间的选择

当创建`上次更新`规则时，您可以使用选择窗口选择日期和时间.

![](/images/image244_detrac.jpg)

您可以使用箭头或通过单击年份和月份来选择年份和月份。
要选择日期，在日历上点击它，
要选择时间，可以使用滚动列表选择小时和分钟。
或者你可以点击`Now`按钮来选择当前的日期和时间。
如需申请，请按`Ok`.

[state]: /docs/manual/basics/vocabulary/#state
[stage]: /docs/manual/basics/vocabulary/#stage
[subset]: /docs/manual/basics/vocabulary/#subset
[resource]: /docs/manual/basics/vocabulary/#resource
[credentials]: /docs/manual/basics/vocabulary/#credentials
[mode]: /docs/manual/basics/vocabulary/#mode
[dimension]: /docs/manual/basics/vocabulary/#dimension
