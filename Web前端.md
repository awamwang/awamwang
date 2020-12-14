# Web前端开发简历

****

| 项目         | 内容                                      | 备注                         |
| ------------ | ----------------------------------------- | ---------------------------- |
| 姓名         | 王蒙                                      |                              |
| 年龄         | 31（1990）                                | -                            |
| 学历         | 本科                                      | -                            |
| 学校         | 西安电子科技大学                          | 一个注重计算机知识的理科学校 |
| 专业         | 信息与计算科学                            | 数学学院                     |
| 期望工作地点 | 成都                                      |                              |
| 当前工作     | 前端开发                                  | 普华永道成都                 |
| Github       | [Github主页](https://github.com/awamwang) |                              |
| 手机         | 19938820324                               |                              |
| 邮箱         | wangnew2013@126.com                       |                              |

## 自我总结

+ 业务能力：专注前端开发，有全栈能力。
+ 业务支持：经验丰富，持续学习，有产品视角。
+ 工作能力：认真负责，解决问题能力强，追求效率。
  【特长】
  效率提升：在效率提升方面有大量经验和实践，例如小工具开发、工作流程优化、Vim使用
  产品与质量意识：有测试和有产品设计经验，有质量意识与方法，能提出产品设计的合理建议

## 技能标签

**`# Web基础`** **`# JavaScript`** **`# Vue`** **`# NodeJs`** **`# Vim`** **`# 效率提升`**

## 工作经历

### 最近工作-PC端Web前端开发（成都）

> 2018.08 - 至今
> 普华永道会计师事务所（成都），咨询行业，千人规模，技术团队50人

#### Workflow for Assurance

**`# Form型页面`** **`# 状态、逻辑判断`**

> PC端：Vue单页 + sass + Element.UI + RESTful API + ECharts
> 【简述】：工作流平台，重状态和逻辑，轻UI。
> <img src="https://awam-image.oss-cn-chengdu.aliyuncs.com/images/%E5%8D%A1%E7%89%87list.jpg" style="zoom: 50%;" />
> 【特点】

- 以Form页面和List页面（包括一些变形的List页面）为主
- 大量使用标签页、弹窗
- 少量报告型页面，使用ECharts

##### Service Type-Translation

**`# 第一个特性`** **`# 计算逻辑`**
【简述】40余个Service Type之一，入职后第一个特性
<img src="https://awam-image.oss-cn-chengdu.aliyuncs.com/images/1606725681427.png" style="zoom: 50%;" />
【特点】

- 根据Form的填写结果，计算时间、提示文字、上传资料内容、难易度
  【产出】
- 计算逻辑、计算配置 + 自动化工具（根据业务Excel配置生成代码配置）（第二版）

##### Service Type-公共

**`# 公共组件抽取`**  
【简述】目前有40+的Service Type，都是复杂度不同的Form表单
【特点】

- Form页面的操作流程大体一致
  【产出】
- 公共组件：抽取公共代码形成支持配置的组件，将各自的Form嵌入公共流程中，加上少量配置，减少Service Type开发的重复工作

#### Workflow for Advisory

**`# 重构`** **`# 组件库`**  

> PC端：Vue单页 + Element.UI + RESTful API
> 【简述】[Workflow for Assurance](#Workflow for Assurance)的兄弟项目
> 【特点】

- UI风格继承老项目
- 本人单独负责前端，从项目初始化到上线维护
- 迁移代码 + 新版Vue脚手架 + 重构 + 组件库 + 新特性
  【产出】
- 新项目模板（工程配置 + 公共代码）
- [组件库](https://github.com/keepgoingwm/element-components.git)（封装Element.UI）

##### 编辑+反显合一的Form组件

【简述】项目中的Form表单大多需要反显（展示），或者部分编辑，所以把填写和展示放到同一组件中
【优点】

- 数据同源、处理方法共用（if-else代码放到组件中、群组的disable、plain属性）
- 样式共用

##### Calendar特性

**`# TypeScript`** **`# 开源代码修改`**

> 开源库 + TypeScript
> 【简述】引用开源第三方库[FullCalendar](https://fullcalendar.io/)，基于其普通版的功能，修改源码新增“Event（一个条目）排序”特性
> <img src="https://awam-image.oss-cn-chengdu.aliyuncs.com/images/calendar.jpg" style="zoom:50%;" />
> 【特点】

- 封装第三方组件，充分利用其功能
- 面向对象编程 + Typescript
  【产出】
- 业务特性
- 增强版的[FullCalendar](https://github.com/super-calendar/fullcalendar.git)

#### Common Service - SPT

【简述】业务架构升级，抽取出公共服务，SPT（Standard Processing Time）是其中一部分
【特点】

- 公共特性，功能相对独立
- 项目管理方式：类monorepo项目，多个Common Service放在同一仓库管理

##### Package配置及Table展示

**`# 最复杂特性`**
【简述】动态配置表单选项与标准用时的计算关系。包括表单选项之间的内在联系，选项选择结果与时间、其他配置项之间的决定与计算关系。
<img src="https://awam-image.oss-cn-chengdu.aliyuncs.com/images/1606741072511.png" style="zoom: 50%;" />
【特点】

- 高灵活性：选项关系、计算公式设置
- 前端逻辑重：关系添加，表格绘制（根据配置的关系），手动实现Radio、Checkbox的选择逻辑；选择项数据提取、保存、反显；从表格中提取出供后端计算的数据格式（首列的特殊性、合并单元格、同行数据拆分）
  【产出】
- 类SDK：包括组件，mixin，样式

### 个人项目

#### vue-number-directive

> Vue plugin + Parcel（构建） + Cypress（测试）+ Travis（CI）+ StoryBook（文档）
> [项目地址](https://github.com/awamwang/vue-number-directive)
> 【简述】以更优雅的方式实现Number Input格式控制

#### vue-wangeditor-awesome

[项目地址](https://github.com/awamwang/vue-wangeditor-awesome)

> Vue 组件
> 【简述】知名富文本编辑器[wangEditor](http://www.wangeditor.com/)的Vue组件封装。

#### koa-route-schema

[项目地址](https://github.com/awamwang/koa-route-schema)

> Koa 插件
> 【简述】支持[jsonschema](http://json-schema.org/)（合法性校验）的Koa route插件。


### 一、软件测试（华为西安）

**`# 质量意识`**

> 2012.07 - 2014.10
> 核心网产品线，传统软件测试（c语言）

```
1. 测试思维，质量、安全意识
2. 自动化测试能力
3. 工作习惯——总结、改进、效率提升
```

离职原因：考研；想转开发岗位


### 二、考研

**`# 失败经验`**

> 2014.10 - 2015.12
> 家人的支持下考研，志愿上海交大，未录取

```
1. 失败经验，自我认知
2. 学习能力提升
```


### 三、移动端Web前端开发（上海信派）

> 2016.3 - 2018.4
> 10人规模创业型公司，信贷行业，自主产品“飞单宝”；外包做微信公众平台开发

#### 你我贷企业微信项目

> 2016.6 - 2017.7（分为2期，中间穿插了其他项目）

1. Vue + vux(UI) + sass，中大型前后端分离单页应用
2. 独立开发前端主要特性——仿朋友圈、考勤管理（打卡页面、报表页面）、成员管理（成员树）、仿红包（发、领）、生日祝福（资源预加载、模板页面）、绩效查询、薪资查询

```
1. Vue1实践，前端基础能力
2. 微信公众号SDK应用
3. vux组件库、vuex状态管理、微信JsSDK、地图、定位、无限加载等技术
```

#### 其他前端项目

> 一些微信公众平台的web项目，技术栈都是vue + sass(less) + vux
> 除玥玛项目为老项目移植，其他项目均为无模板的手工项目
> 前端的参与度均在50%及以上

- 云微粒分销商城类型项目——单独服务截屏 -> 前端截屏，基础的H5视频播放
- 玛丽黛佳轮盘活动页面——单页游戏、状态控制
- 申万宏源股市猜猜猜活动——前后端时间同步、金融数据处理
- 申万宏源全民经纪人项目
- 玥玛商城类型项目
- 金辉投票页面性能优化

#### 其他非前端项目

- 微信机器人服务（后端项目）——Egg.js + Wechaty第三方库
- 征信解析工具——Java
- 贷款产品知识库（规则引擎应用）——Java + Drools；后来版本改用Prolog语言

离职原因：公司发展


## 技能

<strong style="background:green;color:white;"> 精通 </strong> <strong style="background:#00cc00;color:white;"> 熟练 </strong> <strong style="background:#00eeee;color:white;"> 熟悉 </strong>

### 前端技能

| 名称                  | 熟练度                                                       | 备注                                                         |
| --------------------- | ------------------------------------------------------------ | ------------------------------------------------------------ |
| JavaScript            | <strong style="background:green;color:white;"> 精通 </strong> |                                                              |
| Html/CSS              | <strong style="background:#00cc00;color:white;"> 熟练 </strong> | Html标签语义化；CSS布局、基本样式                            |
| Sass                  | <strong style="background:#00cc00;color:white;"> 熟练 </strong> |                                                              |
| Vue                   | <strong style="background:green;color:white;"> 精通 </strong> | 基本语法，熟悉一些较新、底层的使用；<br />了解实现原理<br />全家桶及Element.UI等 |
| React                 | <strong style="background:#00eeee;color:white;"> 熟悉 </strong> | 熟悉基本语法                                                 |
| HTTP                  | <strong style="background:#00cc00;color:white;"> 熟练 </strong> | API调用；跨域；安全；状态码；协议分层                        |
| TypeScript            | <strong style="background:#00cc00;color:white;"> 熟练 </strong> | 熟悉语法；多个项目使用                                       |
| 面向对象编程/设计模式 | <strong style="background:#00eeee;color:white;"> 熟悉 </strong> |                                                              |

### 工程

| 名称             | 熟练度                                                       | 备注                                                    |
| ---------------- | ------------------------------------------------------------ | ------------------------------------------------------- |
| Webpack          | <strong style="background:#00cc00;color:white;"> 熟练 </strong> | loader、插件使用；了解基本原理                          |
| Jenkins/TravisCI | <strong style="background:#00eeee;color:white;"> 熟悉 </strong> | 搭建并使用过Jenkins服务<br />个人项目使用Travis打包发布 |
| 测试框架         | <strong style="background:#00eeee;color:white;"> 熟悉 </strong> | 熟悉前端测试框架的语法与使用                            |

### 其他开发

| 名称               | 熟练度                                                       | 备注                            |
| ------------------ | ------------------------------------------------------------ | ------------------------------- |
| Express/Koa/Egg.js | <strong style="background:#00cc00;color:white;"> 熟练 </strong> | 有小型或者个人项目经验          |
| Node               | <strong style="background:#00cc00;color:white;"> 熟练 </strong> | 小型工具开发经验                |
| 数据库             | <strong style="background:#00eeee;color:white;"> 熟悉 </strong> | SQL基础；关系型数据库的Node调用 |

### 效率方面

| 名称 | 熟练度                                                       | 备注                                         |
| ---- | ------------------------------------------------------------ | -------------------------------------------- |
| 正则 | <strong style="background:#00cc00;color:white;"> 熟练 </strong> | 业务代码和日常操作中经常使用                 |
| Vim  | <strong style="background:#00cc00;color:white;"> 熟练 </strong> | Chrome、VS Code、Markdown编辑器都使用vim模式 |

### 工具开发

Chrome plugin
VS Code plugin
uTools/Quicker 插件
