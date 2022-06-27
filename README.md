# Simple Design for DCBEV App 

## 基本设想
### 用意
App将主要用于完善协会日常的管理， 加强人员之间的互动和交流。并希望以此能够创建一个简洁，透明和公正的管理体系。
### 目前的问题
* 过于依赖微信
* 会员信息变化滞后，不透明
* 理事之们无法及时了解协会很多工作的进展
* 处理微信群，协会没有官方对外的窗口
* 对各种待处理的事情没有一个完整的记录
* 太多工具

### App的功能設想
* 会员管理： 能够增刪查改会员； 能够有简单的会员数量的图表。
* 联赛管理： 能够增刪查改联赛的日期，并且允许会员根据自身情况报名。
* 任务管理： 能够增刪查改各项协会的工作， 工作可以委派给个人，并能更新状态。
* 活动报名： 能够创建各类活动，并允许会员报名。
* 信息发布： 发布协会的情况，入会的要求，联系方式等等。 并且能够及时发布通知。


### App模块
虽然模块的实现方式有差异，还是要尽可能的注意，不要给以后可能的合并制造太多困难。合并可能是双向的，主要看wordpress和自己写的App的稳定性。 暂时的模块结构：

* 会员管理， 联赛管理和任务管理 -> DCBEV App (自己写)
* 活动报名， 信息发布 -> WordPress

### App开发分工
（希望能有更多的人加入，以下的只是我的设想）
* DCBEV App -> DD, PengCC，？
* WordPress -> Eason，？

### App目前进度
* 会员管理：JSON/HTML✅
* 联赛管理：JSON/HTML✅
* 任务管理： 待开始
* 活动报名： 待开始
* 信息发布： 待开始

### Demos
* DCBEV BE + FE -> https://agile-inlet-73564.herokuapp.com
* DCBEV FE -> @PengCC

## 技术工具一览
（不感兴趣的同学可以完全忽略这部分。 有些不知道怎么翻译好，所以就干脆不翻了😉）

### Tech Stack
* Web Server: Nginx
* BE: Node + express + Mongo (Atlas cluster?), SQL for Wordpress?
* FE: vue, pug/jade, Wordpress
* Server: Linux Server (Wordpress plugin?)

### Authentication Layer
* Phase 1: Session Authentication
* Phase 2: Session -> Token (?)

### Responses
Most of the APIs can right now response to both HTML and json. 
* HTML responses for backend rendering
* JSON responses

### Rendering
* Phase 1: Backend rendering + Frontend rendering
* Phase 2: Backend rendering phases out.

#### More
APIs...
