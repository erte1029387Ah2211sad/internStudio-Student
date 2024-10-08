## 1、创建一个开发机，并本地进行连接。
	本地连接时，如果不需要无密码登录，则可以不用配置ssh安全密钥，如有需求，本地进行生成后，传递到开发机的配置上
![Pasted image 20240808154027](../img/Pasted%20image%2020240808154027.png)

## 2、创建 hello_world. Py 文件

	该步骤涉及到了：创建目录命令：mkdir ； 创建文件命令： touch； 编辑文件内容：vim； 查看文件内容：；

![[Pasted image 20240808154226.png]](../img/Pasted%20image%2020240808154226.png)

## 3、启动 hello_world. Py 项目
### 3.1 安装依赖
在运行代码之前，需要先使用`pip install gradio==4.29.0`命令安装以下依赖包，然后在Web IDE的终端中运行了一个`hello_world.py`
![[Pasted image 20240808160714.png]](../img/Pasted%20image%2020240808160714.png)
### 3.2 配置与本地的连接
ssh -p xxxx4 root@ssh.intern-ai.org.cn -CNg -L 7860:127.0.0.1:7860 -o StrictHostKeyChecking=no
	在这中间经历了几个坑，注意事项一：一定记得启动程序。退出开发机后，程序会停止。二、还是使用 vscode 好用一些。
![[Pasted image 20240808164603.png]](../img/Pasted%20image%2020240808164603.png)

## 4、Linux 常用命令
- **创建文件**：可以使用 `touch` 命令创建空文件。
	- 前边创建 hello_world. Py 的时候已经演示。
- **创建目录**：使用 `mkdir` 命令。
	- 创建 OneDay目录时已经演示。
- **目录切换**：使用 `cd` 命令。
	- 最基础命令，已涉及到。
- **显示所在目录**：使用 `pwd` 命令。
- ![[Pasted image 20240808165153.png]](../img/Pasted%20image%2020240808165153.png)
- **查看文件内容**：如使用 `cat` 直接显示文件全部内容，`more` 和 `less` 可以分页查看。
	- 上面操作时已经使用过 cat。
	- More 与 less 可自行使用尝试下。
- **编辑文件**：如 `vi` 或 `vim` 等编辑器。
	- 经典的编辑功能，：wq 保存退出。
- **复制文件**：用 `cp` 命令。
- **创建文件链接**：用 `ln` 命令。
- **移动文件**：通过 `mv` 命令。
- **删除文件**：使用 `rm` 命令。
- **删除目录**：`rmdir`（只能删除空目录）或 `rm -r`（可删除非空目录）。
- **查找文件**：可以用 `find` 命令。
- **查看文件或目录的详细信息**：使用 `ls` 命令，如使用 `ls -l` 查看目录下文件的详细信息。
- **处理文件**：进行复杂的文件操作，可以使用 `sed` 命令。
