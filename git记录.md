# 基本配置
## 查看配置信息
	git config --list
## 编辑配置信息
	git config user.name
	git config user.email

# 基本操作
## 创建仓库
### 初始化
	git init
### 拷贝
	git clone
## 提交与修改
	git add		|	添加文件到仓库
	git status	|	查看仓库当前的状态，显示有变更的文件。
	git diff	|	比较文件的不同，即暂存区和工作区的差异。
	git commit	|	提交暂存区到本地仓库。
	git reset	|	回退版本。
	git rm		|	删除工作区文件。
	git mv		|	移动或重命名工作区文件。

## 提交日志
	git log

# 一般操作流程
## 获取并配置sshkey
	ssh-keygen -t rsa -b 4096 -C a379300239@126.com
## 创建新数据库
	在github上创建
	配置信息
		git config user.name
		git config user.email
	连接数据库
		git remote add orign git@github.com:a379300239/qccSpider.git
## 保存文件
	添加到暂存区
		git add -A .
	提交到本地文件
		git commit -m '备注'
	提交到服务器
		git push orign master