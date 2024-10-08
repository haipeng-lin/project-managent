﻿## 一、关于项目流式管控平台

&emsp;&emsp;项目流式管控平台，是一个智能化管控系统，后端使用了SpringClound  Alibaba、MySQL数据库、Flowable工作流，前端使用了Vue、Echarts、WebSocket等技术。系统实现了项目管理、任务管理、任务审批、成本数据预测、AI聊天等功能。

## 二、系统架构及模块功能

### 1.架构图

<img src="https://haipeng-lin.oss-cn-shenzhen.aliyuncs.com/202409292143870.png" alt="项目流式管控平台架构图" style="zoom: 15%;" />

### 2.模块

&emsp;&emsp;项目流式管控可视化平台分为五大模块：认证模块、项目模块、流程模块、智能模块、可视化模块，

&emsp;&emsp;其中核心模块为**项目模块、流程模块、以及智能模块**

### 3.功能

- **认证模块：** 登录认证、权限认证
- **项目模块：**
	- 项目管理：创建项目，设置项目编号、进度、开始和结束时间
	- 任务管理：创建、分配和追踪任务，设置任务优先级和截止日期
	- 物料管理：项目、任务所需的物料设备管理
	- 项目培训：分为培训计划、培训确认两个阶段
	- 项目验收：对项目的各个功能进行验收
- **流程模块：**
	- 流程设计：使用Flowable工作流，设计任务审批流程
	- 任务提醒：集成邮件和钉钉，实现任务审批消息提醒

- **智能模块：**
	- 机器学习：使用机器学习模型分析以往项目的花费数据，预测当前项目的成本，帮助资金分配
	- 智能聊天：接入星火讯飞模型，制作聊天页面，协助团队成员获取项目管理知识的常见定义、问题

- **可视化模块：**

	- 项目/任务进度：集成Echarts，可查看项目进度、任务进度

	- 完成效率：统计各个项目和任务完成时间、效率

	- 甘特图：自动生成项目甘特图，支持导出Excel
