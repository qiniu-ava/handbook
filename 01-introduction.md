# 概述

本小节对 AVA 平台做一个概要性的介绍.

在传统的深度学习过程中,用户需要管理一切细节,包括数据的存储,数据的处理,分布式平台的搭建,docker镜像管理,模型输出/评估/发布等一切细节.这种过程耗时长,繁重并且比较容易出错,并且模型训练出来后不能及时的发布应用.

AVA平台是七牛人工智能实验室打造的一款为深度学习提供定制服务的平台,包括数据管理,镜像管理,训练框架管理,训练任务管理,模型管理等.主要目的是优化资源管理,把算法研究员和开发员从繁琐的资源管理和环境管理中解脱出来,让他们能聚焦于算法和模型本身的设计和实现.同时,提供完整的深度学习方案,让不熟悉深度学习算法的用户可以快速方便的使用平台的功能,快速输出深度学习的结果.

且AVA是构建在七牛云存储服务（KODO）之上的,实现所有数据管理和落地都在云端,同时拥有管理和对接其他云存储服务的能力；有效管理 GPU 资源,通过合理划分和调度,将调试代码与模型训练分开进行,充分利用 GPU 资源,减少GPU闲置时间；最关键的是实现了存储和计算分离,使得各自可以独立平行扩展.

AVA提供了一个公共的训练平台,七牛的AI应用大部分都运行在该平台上,经过多次训练迭代,得到成熟的模型,然后提供对外的产品服务.平台的主要功能模块包括数据集、工作台、训练、模型和镜像等,用户可在之后的章节内了解对应的概念,并且快速启动一个训练.通过 AVA 平台,用户可以快速的执行完整的深度训练流程,包括导入训练数据,方便的使用常用的深度学习框架,一键启动深度训练任务,快速导出训练模型等.

要使用AVA平台进行深度学习训练,请注册七牛云portal账号,再申请AVA深度学习平台的使用权限.详细： 04 AVA 申请注册流程