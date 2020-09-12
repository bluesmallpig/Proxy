## Loon 教程

此文件夹内存放 Loon 使用教程，请仔细阅读免责声明，任何一经点击教程内文档的阅读者便视为您已接受此免责声明

------

### 免责声明

- 此教程仅供正版购买 Loon 的用户学习如何使用 Loon 这款软件，chiupam 从未提供机场服务或教唆大陆用户擅自建立、使用非法定信道进行国际联网

- 用户通过此教程利用 Loon 使用非法信道进行国际联网并实施违反国家或地区法律法规的行为，对此类用户造成的行为后果，chiupam 概不负责

- 教程内只教授配置脚本功能的方法，不提供任何具体的损害自然人、法人、非法人组织的合法利益的脚本

- 请勿将脚本用于任何商业用途或者非法目的，对此造成的任何后果，chiupam 概不负责

- 任何以任何方式阅读此教程的、直接或间接操作此教程内步骤的阅读者都应仔细阅读此声明。chiupam 有权更改、补充此免责声明的权利，任何一经点击教程内文档的阅读者便视为您已接受此免责声明

------

### 配置栏篇

目的在于提高用户自定义 Loon 配置的能力，按 `配置` 栏面板顺序编写教程

#### 节点

- [单个节点](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Proxy.md)（手动添加代理节点）

- [订阅节点](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Remote_Proxy.md)（订阅一个节点合集，通常是用户购买的机场提供）

- 筛选订阅节点（将订阅节点筛选成用户需要的代理节点，减少过多代理节点出现在策略组内，方便用户选择需要的代理节点）

  - [正则表达式](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Regex.md)（掌握基本的正则表达式写法）

  - [筛选类型为 `NodeSelect` 的筛选方法](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Remote_Filter_NodeSelect.md)（手动筛选节点）
  
  - [筛选类型为 `NameKeyword` 的筛选方法](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Remote_Filter_NameKeyword.md)（利用关键词筛选订阅节点，但不能排除节点，适用于不会写正则表达式的用户）

  - [筛选类型为 `NameRegex` 的筛选方法](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Remote_Filter.md)（利用正则表达式筛选订阅节点）

- [节点与策略组之间的嵌套](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Remote_Proxy_in_Proxy_Group.md)（将代理节点添加到策略组下）

#### 策略

- 没有默认代理策略组的 Loon 

  - [代理策略组](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Default_Proxy.md)（理解什么是代理策略组，搭配 `对全局策略的理解` 教程）

  - [对全局策略的理解](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Global_Group.md)（全局代理必须需要搭配全局策略使用的原因）
  
- [新建策略组](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/New_Proxy_Group.md)（手动添加一个策略组，注意此处是子策略组）

- 母策略组与子策略组之间的逻辑关系

  - [正确分辨母策略组和子策略组](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/TOP_Policy.md)

  - 理解 `俄罗斯套娃` 的小把戏 —— [子母策略组之间的嵌套](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Matryoshka.md)

- 常用的三种自动策略组 

  - [URL-Test 策略组的设置](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/URL-Test.md)（优选最低延迟）
  
  - [Fallback 策略组的设置](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Fallback.md)（健康检测）
  
  - [PCC 策略组的设置](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/PCC.md)（相同主机名锁定同一节点）
  
  - SSID策略组（不写此教程是因为SSID策略组在 Loon 有逻辑问题，需要等待开发者修改逻辑关系）
  
#### 规则

- [何为规则](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Ruld_Summary.md)（代理软件中设计规则的原因）

- [单个规则](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Rule.md)（通过 UI 手动添加一个本地规则）

- [订阅规则](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Remote_Rule.md)（订阅一个规则合集并选择母策略组）

- [Final规则](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Final.md)（本地规则与远程规则都无法匹配访问请求所走规则情况下的兜底条款）
 
#### 复写

- [订阅复写](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Remote_Rewrite.md)（未写）（主要功能为去除各类 APP 广告，但是不确保完全去除广告）

#### 脚本

- [基础 cron 表达式的学习](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/cron.md)（修改定时脚本的执行时间）

- 在 Loon 中使用脚本（从入门到放弃）

  - [入门 —— 如何看懂三种脚本语句的必备格式](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/JaveScript_Format.md)（必看，初次使用脚本功能的用户认真阅读并充分理解）

  - [初级 —— 如何看懂一个脚本配置代码](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/JaveScript_1.md)（解开用户对于脚本问题的困惑）

  - [中级 —— 如何将脚本配置代码写入 Loon 内发挥作用](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/JaveScript_2.md)（让 Loon 真正执行脚本的必备操作）
  
  - 高级 —— ?????? （未构思）
  
  - [放弃 —— 如果用户仍然不懂如何操作](https://t.me/chiupam)（天知道哪个大佬能救得了这种用户，亲们，这边提供有偿代写配置，收费标准：150元/次）

- [添加脚本文件 —— 从URL下载](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Download_From_URL.md)（利用 `从URL下载脚本` 功能并将脚本下载存储在 `iCloud` 中）

- 本地脚本（通过 UI 方法添加脚本）

  - [添加本地路径脚本](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Local_JaveScript.md)（脚本位置选择 `Local` ，需要搭配 `添加脚本文件 —— 从 URL 下载` 教程学习）
  
  - [添加远程链接脚本](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Remote_JaveScript.md)（脚本位置选择 `Remote` ）
  
- [修改本地脚本设置](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/JaveScript_Modify.md)（修改本地脚本的别名、cron表达式、脚本位置等系列操作）

- 订阅脚本（懒人神器）

  - [订阅脚本中对 URL 的要求及内容格式要求](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Remote_Script_Format.md)（必看，否则新手用户极易出现订阅脚本返回无脚本的错误情况）

  - [添加订阅脚本](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Remote_Script.md)（了解订阅脚本功能的作用，以及订阅的 URL 的链接要求和内容要求）

  - [创建单个本地分支](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Branch.md)（将订阅脚本内需要的脚本移到本地脚本中，不可修改本地脚本内容，仅可修改 cron 表达式）
  
  - [创建单个本地分支并拷贝js](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Branch&Copy.md)（将订阅脚本内需要的脚本移到本地脚本中，可修改脚本内容，也可修改 cron 表达式）

#### DNS（本人不懂，直接跳过此教程）

- DNS服务器

- DNS映射

#### 插件

- [初步了解插件功能](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Plugin_Summary.md)（强大的自定义配置神器）

- [添加插件中中对 URL 的要求及内容格式要求](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Plugin_Format.md)（必看，否则新手用户极易出现各种奇怪的错误情况）

- [添加插件](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Plugin.md)（如何添加一个插件）

- [推荐插件 URL](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Plugin_Recommend.md)（为新手用户整理的实用性插件，教程内提供 URL 地址）

#### MITM

- [域名](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/hostname.md)（添加域名的两种方法）

- [证书管理](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Certificate.md)（出现关于证书类弹窗的原因以及解决方法）

#### 编辑

- [文本编辑](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Configuration.md)（Loon 的配置文件）

#### 更多

- [网络共享](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Network_Sharing.md)（可为处于同一 WiFi 下的设备实现科学上网）

---

### 作者声明

- 为了读者的方便，禁止将此教程 **链接** 或 **内容** 转发至大陆内任何社交平台上，如果发现，chiupam 将删库处理

- 教程编写中，确有高度需求的教程请前往 [Telegram Loon 官方群](https://t.me/Loon0x00) 并 @[chiupam](https://t.me/chiupam) 提出，chiupam 会安排时间加快写出教程

- 非专业人员，如果用户查阅教程后仍不能解决用户的问题，可以前往 [Telegram Loon 官方群](https://t.me/Loon0x00) 并进行友好交流

- 精力有限，义务编写教程，不可能即时更新用户需要的教程

- 智力水平有限，对于自身也无法解决的问题，不可能编写此类教程

