
## git
> 版本控制器

+ 网址 https://git-scm.com/downloads

### 基本命令
+ 在文件夹内 输入 git init  初始化仓库
+ git status 查看文件是否被暂存或存储 ,不是必须的命令
+ git add . 把文件存入暂存区
+ git commit -m'xxxx'  把文件存入到存储区  -m'xxx'不能忘

+ 添加远程源将本地仓库和远程仓库建立连接
```
	//nevermo2013/noteH5.git 每个人不同 看个人设置
	git remote add origin https://github.com/nevermo2013/noteH5.git
```
+ git push -u origin master  把本地文件提到到远程github
+ 第二次暂存 提交  后 不需要再配置源信息,提交只需要Git push即可


## github
> 前端最重要的网站.

+ 网址 https://github.com/
+ 点击右上角 +  new  repository
+ 重要: Repository name不能写中文
+ 不要勾选 "Initialize this repository with a README" 
