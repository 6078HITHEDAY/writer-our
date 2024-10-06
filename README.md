# writer-our
## 仓库说明
* 用GitHub来同步小说有点大材小用了
* 但也不是不能用😄
## 小说说明
* 仙界☯️🛐✝️🔯✡️
* 科学⚛️
## 文件夹说明
* 设定文件夹📁为设定（世界观，角色）
* 章节文件夹📁为章节
## 全部使用md语法
* 不会去菜鸟教程学习

## 部署指南
### Android部署
这里🈁采用termux，一个简单的Linux终端
* 安装**termux**
[GitHub - termux/termux-app: Termux - a terminal emulator application for Android OS extendible by variety of packages.](https://github.com/termux/termux-app)
* 换源
[termux清华源](https://mirrors.tuna.tsinghua.edu.cn/help/termux/)
* 安装git
```
pkg install git
```
* 在 Termux 中配置 Git 与在其他命令行工具中基本相同，以下是在 Termux 中配置 Git 的简单步骤：

首先，在 Termux 中打开一个新的终端窗口。
* 输入以下命令以设置用户名称，将 "Your Name" 替换为你的 GitHub 用户名：
```
git config --global user.name "Your Name"
```
* 输入以下命令以设置用户邮箱，将 "your_email@example.com" 替换为你的 GitHub 注册邮箱：

```
git config --global user.email "your_email@example.com"
```
* 如果你进行代码编辑时希望使用 Vi 编辑器，你可以设置 Git 默认使用 Vi 编辑器：
```
git config --global core.editor "vim"
```
### 使用 SSH 连接到 GitHub
* 生成 SSH 密钥对：
```
ssh-keygen -t rsa -b 4096 -C "your_email@example.com"
```
* 在这里替换 "your_email@example.com" 为你在 GitHub 上注册的邮箱地址。然后系统会提示你选择密钥保存的位置和设置密码等信息。
* 在 GitHub 上添加 SSH 公钥：
```
 cat ~/.ssh/id_rsa.pub
```
* 复制你的 SSH 公钥，一般是在  ~/.ssh/id_rsa.pub  文件中。
登录到 GitHub 上，点击头像 -> Settings -> SSH and GPG keys -> New SSH key，将你的 SSH 公钥粘贴进去。
* 测试 SSH 连接：
```
ssh -T git@github.com
```
### 克隆仓库到本地
