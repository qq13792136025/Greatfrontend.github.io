---
layout: post
title: 概念模型、逻辑模型、物理模型的区别
category: star
tags: Concept
description: 浅显介绍一下三者的区别，自己一个记录
---

## 概念模型

概念数据模型（Conceptual Data Model）：简称概念模型，主要用来描述世界的概念化结构，它使数据库的设计人员在设计的初始阶段，摆脱计算机系统及DBMS的具体技术问题，集中精力分析数据以及数据之间的联系等，与具体的数据管理系统（Database Management System，简称DBMS）无关。概念数据模型必须换成逻辑数据模型，才能在DBMS中实现。

概念数据模型是最终用户对数据存储的看法，反映了最终用户综合性的信息需求，它以数据类的方式描述企业级的数据需求，数据类代表了在业务环境中自然聚集成的几个主要类别数据。

概念数据模型的内容包括重要的实体及实体之间的关系。在概念数据模型中不包括实体的属性，也不用定义实体的主键。这是概念数据模型和逻辑数据模型的主要区别。

概念数据模型的目标是统一业务概念，作为业务人员和技术人员之间沟通的桥梁，确定不同实体之间的最高层次的关系。

在有些数据模型的设计过程中，概念数据模型是和逻辑数据模型合在一起进行设计的。

## 逻辑模型

逻辑数据模型（Logical Data Model）:简称数据模型，这是用户从数据库所看到的模型，是具体的DBMS所支持的数据模型，如网状数据模型(Network Data Model)、层次数据模型(Hierarchical Data Model)等等。此模型既要面向用户，又要面向系统，主要用于数据库管理系统（DBMS）的实现。

逻辑数据模型反映的是系统分析设计人员对数据存储的观点，是对概念数据模型进一步的分解和细化。逻辑数据模型是根据业务规则确定的，关于业务对象、业务对象的数据项及业务对象之间关系的基本蓝图。

逻辑数据模型的内容包括所有的实体和关系，确定每个实体的属性，定义每个实体的主键，指定实体的外键，需要进行范式化处理。

逻辑数据模型的目标是尽可能详细的描述数据，但并不考虑数据在物理上如何来实现。

逻辑数据建模不仅会影响数据库设计的方向，还间接影响最终数据库的性能和管理。如果在实现逻辑数据模型时投入得足够多，那么在物理数据模型设计时就可以有许多可供选择的方法。

## 物理模型

物理数据模型（Physical Data Model）:简称物理模型，是面向计算机物理表示的模型，描述了数据在储存介质上的组织结构，它不但与具体的DBMS有关，而且还与操作系统和硬件有关。每一种逻辑数据模型在实现时都有起对应的物理数据模型。DBMS为了保证其独立性与可移植性，大部分物理数据模型的实现工作又系统自动完成，而设计者只设计索引、聚集等特殊结构。

