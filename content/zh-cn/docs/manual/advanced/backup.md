---
title: '备份任务和项目'
linkTitle: '备份'
weight: 17
---

## 概述

在标注平台上，您可以备份任务和项目。
这可以用于备份您PC上的任务或项目，或传输到另一台服务器.

## 创建备份

要备份任务或项目，请打开操作菜单并选择“备份任务”或“备份项目”。.

![](/images/image219.jpg)

(可选) 在`自定义文件名`文本字段中指定备份文件名称,
否则备份项目的文件名称将由掩码 `project_<项目名>_backup_<日期>_<时间>.zip`给出
备份任务的文件名`task_<任务名>_backup_<日期>_<时间>.zip`.

![](/images/image253.jpg)


## 从备份中创建

要从备份创建任务或项目，请转到任务或项目页面,
单击`从备份创建`按钮并选择所需的存档.

![](/images/image220.jpg)

结果，您将得到一个任务，其中包含先前导出的任务的数据、参数和标注.

## 备份文件结构

结果，你会得到一个包含数据的zip存档,
任务或项目，任务规范和标注具有以下结构:

{{< tabpane >}}
  {{< tab header="任务备份结构" >}}
    .
    ├── data
    │   └── {用户上传的数据}
    ├── task.json
    └── annotations.json
  {{< /tab >}}
  {{< tab header="项目备份结构" >}}
    .
    ├── task_{id}
    │   ├── data
    │   │   └── {用户上传的数据}
    │   ├── task.json
    │   └── annotations.json
    └── project.json
  {{< /tab >}}
{{< /tabpane >}}
