---
title: '训练步骤'
linkTitle: '训练步骤'
weight: 5
description: '从创建项目到训练到验证的训练步骤.'
---


- [创建项目](#创建项目)
- [快速创建任务](#快速创建任务)
- [进行标注](#进行标注)
- [开始训练](#开始训练)


## 创建项目
创建项目.具体请参阅[创建项目][create-project]
   > **备注**:因为需要该项目的数据参与训练,故创建项目时最好填写检修保存路径以及用户名和密码(用于快速创建任务)，选择设备和工序/表面<br>
   > 各种工序所使用的标签的Json源码格式请现场AI实施人员给予
   > 检修保存图片路径、主机用户名以及共享密码将被遗弃

   ![](/images/image_device.jpg)

## 快速创建任务
   > (将被移除，请使用[手动创建任务][create-task], 一定要指定项目)
1. 设置检修软件AOI是`AI工序选择` AVI是`AI膜面选择`,只有设置了才会导出图片
   ![](/images/image_model_attr.jpg)
2. 检修软件导出所需图片,导出路径为`参数设置->缺陷报告`路径下的`Dataset文件夹`的以AI工序选择的名称命名的文件夹内
   - `F7`判定所选图片为漏失并导出到路径中的`aoi_missing`文件夹中
   - `F8`判定所选图片为误判并导出到路径中的`aoi_wrong`文件夹中
3. 在项目页面上`动作`菜单里点击`快速创建任务`按钮,
    就会选择从检修导出的图片上传到服务器并创建任务,任务命名默认为当前日期
![](/images/quick_create_task.jpg)

> **备注** 从项目快速创建任务取决于项目的工序或膜面,比如,如果项目的工序是`内层`,则`快速创建任务`所选的图片是从`{导出路径}/内层`中读取所有图片,如果没有图片,则会提示错误

## 进行标注
标注请参考
- [使用矩形标注](/docs/manual/advanced/annotation-with-rectangles/)
- [使用多边形标注](/docs/manual/advanced/annotation-with-polygons/)

标注完成之后在标注界面的`菜单`点击`完成作业`

## 创建训练任务
要创建新训练任务，请打开训练任务配置:
![](/images/create_trainer.png)

并指定以下参数:
1. 在**名称**字段, 输入新任务的名称.
![](/images/trainer_name.png)
2. 指定模型并选择任务
![](/images/trainer_model.png)
3. 选择主机以及相应的显卡（单机多卡训练）
![](/images/trainer_devices.png)
4. 训练参数
   1. **训练批次**： 分批读取数据集的批量大小
   2. **图像尺寸**： 用于训练数据的图像尺寸
   3. **训练周期**： 选择深度学习训练次数,训练轮数越多,通常学习越深,但到了一定轮数就会有极限，并且容易过拟合

进入[训练任务详情](/docs/train/train-details)进行训练


[create-project]: /docs/manual/advanced/projects/#创建项目
[create-task]: /docs/manual/basics/create_an_annotation_task