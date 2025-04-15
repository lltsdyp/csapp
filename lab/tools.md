# INTRO TO BASIC TOOLS

## GDB

### 基本命令
- **`gdb <程序名>`**：启动调试会话  
  `gdb ./a.out`
- **`break <行号/函数名>`**：设置断点  
  `break main`  `break 20`
- **`run`**：启动程序执行

### 断点管理
- **`info breakpoints`**：查看所有断点
- **`delete <断点编号>`**：删除断点  
  `delete 2`
- **`disable/enable <编号>`**：禁用/启用断点

### 执行控制
- **`next`**：单步执行（跳过函数）
- **`step`**：单步进入函数
- **`continue`**：继续执行到下一个断点

### 查看信息
- **`print/FMT <变量>`**：打印变量值  
  `print x`
- **`disassemble <函数名>`**： 反汇编函数
- **`info registers`**：查看寄存器
- **`x/FMT <地址>`**：查看内存
- **`backtrace`**：查看调用栈
- **`frame <编号>`**：切换栈帧

调试时可以使用命令缩写来简化输入：如`c`是`continue`的缩写

教程：
[Beej's Guide](https://beej.us/guide/bggdb/)

---

## Vim

### 模式切换
- **`i`**：进入插入模式
- **`ESC`**：返回普通模式
- **`:`**：进入命令模式

### 移动操作
- **`h/j/k/l`**：左/下/上/右移动
- **`0/$`**：跳转到行首/行尾
- **`gg/G`**：跳转到文件首/尾

### 编辑命令
- **`dd`**：删除当前行
- **`yy`**：复制(yank)当前行
- **`p`**：粘贴
- **`u`**：撤销操作

### 文件操作
- **`:w`**：保存文件
- **`:q!`**：强制退出不保存
- **`:wq`**：保存并退出

vim入门教程：

试试在命令行输入
``` bash
$ vimtutor
```

或者一个很好的在线教程：
[Learn Vim](https://github.com/iggredible/Learn-Vim)

---

## Git

### 仓库操作
- **`git init`**：初始化新仓库
- **`git clone <url>`**：克隆远程仓库  
  `git clone https://github.com/user/repo.git`

### 基本工作流
- **`git add <文件>`**：添加文件到暂存区  
  `git add .`（添加所有修改）
- **`git commit -m "消息"`**：提交更改
- **`git status`**：查看当前状态

### 分支管理
- **`git branch`**：显示分支列表
- **`git checkout -b <分支名>`**：创建并切换分支
- **`git merge <分支名>`**：合并指定分支到当前分支

### 远程操作
- **`git fetch`**：拉取远程分支
- **`git pull`**：拉取远程更新(`git fetch` + `git merge`)
- **`git push origin <分支名>`**：推送本地提交
- **`git remote -v`**：查看远程仓库地址

### 版本追溯
- **`git log`**：查看提交历史
- **`git diff`**：查看文件差异
- **`git reset --hard <commit_id>`**：回退到指定版本

git入门：
[Visualize learning](https://learngitbranching.js.org/)
[Pro Git 2nd Edition](https://git-scm.com/book/en/v2)

---

最后，一个帮助你快速掌握常用编程工具的教程
[Missing semester](https://missing-semester-cn.github.io/)
