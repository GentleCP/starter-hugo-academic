---
title: UCAS-Helper
date: 2023-08-24T11:07:24.147Z
summary: 国科大（UCAS, ucas）校园网登录、课程资源下载、自动评教和分数查询助手
draft: false
featured: true
authors:
  - admin
links:
  - url: https://github.com/GentleCP/UCAS-Helper
    name: Github
    icon_pack: fab
    icon: github
image:
  filename: https://github.com/GentleCP/UCAS-Helper/raw/v2/img/2-1.png
  focal_point: Smart
  preview_only: false
---
# UCAS Helper(一个让UCASer愉悦的小助手)
[![Hits](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2FGentleCP%2FUCAS-Helper&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=hits&edge_flat=false)](https://hits.seeyoufarm.com)
![python version](https://img.shields.io/badge/python-3.5%2B-blue)
![demo version](https://img.shields.io/github/v/tag/GentleCP/UCAS-Helper?color=red)
![license](https://img.shields.io/badge/license-GNU%20v3-yellowgreen)
```angular2
*********************************************************************************
**      #   #   ###     #       ###    #  #   ###  #     ###    ###  ####      **
**      #   #  #       # #     #       #  #  #     #     #  #  #     #   #     **
**      #   #  #      #   #    ####    ####  ###   #     ###   ###   ####      **
**      #   #  #     #######      #    #  #  #     #     #     #     #  #      **
**       ###    ### ##     ##  ###     #  #   ###  ##### #      ###  #   #     **
**                            copyright@GentleCP                               **
**                            version: x.x.x                                   **
**                github: https://github.com/GentleCP/UCASHelper               **
**                            1:course sources download                        **
**                            2:wifi login                                     **
**                            3:wifi logout                                    **
**                            4:course assess                                  **
**                            5:query grades                                   **
**                            q:exit                                           **
*********************************************************************************
```
目录
=================
   * [前言](#前言)
   * [1. 功能介绍](#1-功能介绍)
   * [2. 更新日志](#2-更新日志)
   * [3. 作者信息](#3-作者信息)
   * [4. 效果预览](#4-效果预览)
   * [5. 使用教程](#5-使用教程)
   * [6. 问题反馈](#6-问题反馈)

# 前言
原本只是一时兴起，为了方便写的UCAS课程网站小助手，帮助我自己进行课程资源快速同步。没想到后面随着功能的增加，项目也变得小有规模起来，因此将其开放给全体UCAS同学，小助手的使用方式在下面有介绍，十分简便（需要一点对`python`环境的了解，百度`python`的安装即可），如果你觉得本项目对你有所帮助的话，希望你能帮我点个star，算是对作者的一点激励吧～ 感谢每一个为项目点上`star`，让更多人看到这个项目的人。❤️

# 1. 功能介绍
- [x] 课程资源同步
- [x] 课程评教
- [x] 成绩查询
- [x] 校园网登录/登出
- [x] 校园网账号破解

>  `校园网`相关功能因缺乏校园网环境无法维护确认，感兴趣的可以提交PR:)

[点击这里](https://github.com/GentleCP/UCAS-Helper/raw/v2/docs/functions.md)查看详细功能介绍

# 2. 更新日志
[点击这里](https://github.com/GentleCP/UCAS-Helper/raw/v2/docs/change_log.md)查看更新日志

## 2.1 公告（important）
> 当作者发现或有人提供`UCAS-Helper`的核心功能出现问题时（多半是课程网站改动导致），会在此处加以说明，并提示在哪个版本中修复了该问题，你也可以在[ChangLog](https://github.com/GentleCP/UCAS-Helper/raw/v2/docs/change_log.md)中查看具体的信息

- 【220501】：5.1假期第二天上Github突然发现有人提交了[issue](https://github.com/GentleCP/UCAS-Helper/issues/27) ，没想到这么久了这个项目还有人在活跃使用，因此假期无事正好解决一下存在的小问题，版本更新到2.4.0，现在不支持从`settings.py`中获取用户信息，请将用户信息填写到`conf/user_config.ini`中！当天测试**资源下载、分数查询**功能均可正常使用，希望后续依然有热心的同学能积极提交PR，帮助维护本项目~最后，祝大家5.1劳动节快乐（虽然真正只放了半天QAQ）
  
- 【220328】：PR更新了新的SEP密码登陆方式，于22/3/28功能正常

- 【210528-停更公告】：由于精力有限，作者本人不再进行`UCAS-Helper`的更新维护工作，下面是一些停更后可能会有的问题，在此提前解答。
  - **停更后UCAS-Helper还能用吗**：经本人停更当天`210528`测试，`UCAS-Helper`的**课程网站登录，课程资源同步下载，成绩查询**功能均可正常使用，**校园网登录/登出/破解**功能因本人缺乏校园网环境无法测试，**自动评教功能**由于本人无课程可评亦无法测试（感谢Jingyi Shi对评教功能的修复）。后续若课程网站改动（可能性较小），可能会导致某些功能失效，不管怎样，你可以先尝试`clone`代码使用看看。
  - **还有可能更新吗**：`UCAS-Helper`是一个完全开源的项目，虽然作者不再更新，但依然会接受各个对本项目有用的PR（如修复Bug，添加功能），欢迎有能力、有开源精神的同学`fork`本项目，并提交PR维护。当然，这不是一个**强制**的选项，你也可以`fork`后自己修改个人使用。

- 【210505-分支暂停维护】：⚠️目前由于本人精力原因，项目`master`分支暂时无力维护，请使用稳定版分支`v2`（已修改为默认分支）代码
- 【210414-课程网站登录失效】：由于课程网站改版，之前的登录接口即便账号密码输入正确，依然会提示账号密码错误，该问题已在`v2.3.4`中得到修复，请使用`>=`该版本的程序

# 3. 作者信息

[@GentleCP](https://github.com/GentleCP)

## 贡献者
> 感谢以下同学为项目提供的PR，欢迎更多同学为项目提供贡献

- [waruto210](https://github.com/waruto210)
- [enochii](https://github.com/enochii)
- [shijy16](https://github.com/shijy16)
- [xuzheliang135](https://github.com/xuzheliang135)

# 4. 效果预览

- 小白使用窗口  
    ![](https://github.com/GentleCP/UCAS-Helper/raw/v2/img/2-1.png)
- 自动登录校园网  
    ![](https://github.com/GentleCP/UCAS-Helper/raw/v2/img/3-1.png)
- 校园网账号破解  

- 自动查分  
    ![](https://github.com/GentleCP/UCAS-Helper/raw/v2/img/4-1.png)
- 显示本学期课程列表  
    ![](https://github.com/GentleCP/UCAS-Helper/raw/v2/img/1-1.png)
    
- 同步所有课程资源到本地  
    ![](https://github.com/GentleCP/UCAS-Helper/raw/v2/img/1-2.png)
- 同步指定课程的资源到本地      
    ![](https://github.com/GentleCP/UCAS-Helper/raw/v2/img/1-3.png)
- 同步指定课程的指定一个资源到本地  
  
- 自动评估课程和教师  
    ![](https://github.com/GentleCP/UCAS-Helper/raw/v2/img/5-1.png)

# 5. 使用教程

[点击这里](https://github.com/GentleCP/UCAS-Helper/raw/v2/docs/usage.md)查看使用教程

# 6. 问题反馈
- `issue`：提交前请先确认是否已有相似的`issue`，尝试自己解决。
- 提问方式：请详细描述你遇到的问题，具体包括:
    1. 使用的版本（绝大多数问题通过更新到最新版本可以解决）
    2. 产生问题的功能（哪个具体功能出现了使用问题）
    3. 问题的具体描述（例如**分数查询时长时间卡顿，没有显示结果**，最好配上截图）

如果你发现了问题，并自己解决修复了，希望你能提交PR，作为贡献者帮助完善这个项目。
