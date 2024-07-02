---
title: '完整的组织工作流程指南'
linkTitle: '完整的组织工作流程指南'
weight: 2
---

欢迎使用宜美智AI自训练系统，此页面是您的团队使用计算机视觉标注工具开始标注以及使用宜美智AI模型训练过程的地方。

本指南旨在为您的组织提供有效使用 宜美智AI自训练系统 所需的知识和最佳实践。

我们将引导您完成 宜美智AI自训练系统 工作流程的每个步骤，从初始设置到高级功能。

参阅:

- [工作流图表](#工作流图表)
- [组织的端到端工作流程](#组织的端到端工作流程)

## 工作流图表

工作流程图从高层次概述了一般流程.

[![工作流图表](/images/ymz-workflow-bpmn.png)](/images/ymz-workflow-bpmn.png)

## 组织的端到端工作流程

要在您的组织内使用宜美智AI自训练系统，请按照以下步骤操作:

1. [`在系统上创建一个帐户`](/docs/manual/basics/registration).
2. [建立 **组织**](/docs/manual/advanced/organization).
3. 切换到您创建的**组织**.
4. ["邀请成员加入 **组织**"](/docs/manual/advanced/organization#invite-members-into-organization) 并
   受邀成员分配 [用户角色](/docs/manual/advanced/iam_user_roles).
5. ["创建 **项目**"](/docs/manual/advanced/projects).
6. 创建 [**任务**](/docs/manual/basics/create_an_annotation_task)
   <br>在此步骤中，自训练系统将自动创建作业.
7.  通过将标注人员名称添加到**分配**将任务分配给标注人员
    并将 [**作业阶段**](/docs/manual/advanced/iam_user_roles#job-stage)
    更改为 **标注**.
8.  标注人员将看到分配的作业并对其进行标注.
9.  通过将质检人员名称添加到**分配**将任务分配给质检人员 并将
    [**作业阶段**](/docs/manual/advanced/iam_user_roles#job-stage)
    更改为 **质检**.
10. 质检人员将看到分配的作业并报告问题。
    <br>请注意，质检人员可以纠正问题，请参阅 [**质检**](/docs/manual/advanced/review)
11. 检查问题，如果需要进一步改进，则将工作重新分配给验证人员或标注人员.
12. (可选) [**训练**标注数据](/docs/train/train-process#开始训练)
13. (可选) 训练完模型之后，可以[**验证**训练模型](/docs/train/valid)
14. [**导出数据**](/docs/manual/advanced/export-import-datasets#导出数据集).