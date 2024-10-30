---
title: git账号切换
published: 2024-10-30
description: vscode git账号切换
image: ''
tags: 
    - MAC
    - git 账号切换
category: 开发工具
draft: false 
abbrlink: 5db07504
---

# git账号切换
- 打开VS Code并进入项目目录：
- 打开VS Code，并确保已经进入想要切换Git账号的项目目录。
- 打开终端：
   >通过菜单栏选择“视图”->“集成终端”，或者使用快捷键（如**Ctrl+\`**，Windows和Linux系统；或**Cmd+\`**，Mac系统）来打开终端。
- 查看当前Git配置：
  >输入命令`git config --list`来查看当前的Git配置信息，包括用户名和邮箱。
- 取消当前Git配置（如果需要）：
  >如果要完全取消当前的Git配置，可以使用命令`git config --global --unset user.name`和`git config --global --unset user.email`来删除全局的用户名和邮箱配置。
- 设置新的Git配置：
  >使用命令`git config --global user.name "Your New Username"`和`git config --global user.email "yournewemail@example.com"`来设置新的全局Git用户名和邮箱。这里的“Your New Username”和“yournewemail@example.com”需要替换为实际的新用户名和邮箱。
- 验证新的Git配置：
  >再次使用`git config --list`命令来验证新的Git配置是否已生效。

>**注意**：以上步骤是针对全局Git配置的。如果只想为特定项目切换Git账号，可以在项目目录中打开终端，并省略`--global`参数来设置项目级别的Git配置。