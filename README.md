This is a git repo


## – 如何验证Ubuntu上是否安装Git以及在何处安装Git  
参见[文献1][1]  
```
git --version
```
## - 在Ubuntu上安装和使用Git和GitHub  
参见[初学者指南：在Ubuntu上安装和使用Git和GitHub](https://zhuanlan.zhihu.com/p/44181150)  
1. 下载并安装 Git：  
```
sudo apt-get install git
```  
  
2. 配置 GitHub  
```
git config --global user.name "user_name" # 填github的帐号
git config --global user.email "email_id" # 填github的密码
```  
3. 创建本地仓库  
```
git init Mytest # 如果目录被成功创建（举例，例如建立叫“Mytest”的文件夹），你会看到如下信息：Initialized empty Git repository in /home/akshay/Mytest/.git/
cd Mytest
```  
或者

```
cd ~/Document/dockerfiles # cd到指定文件夹位置
git init
```  
4. 新建一个 README 文件来描述仓库
```
gedit README.md
```
或
```
touch Readme
```
5. 提交（对刚刚的更改进行提交）
```
git add README # 添加索引

git commit -m "some_message" # 提交改动 ；  “some_message” 在上面的命令里可以是一些简单的信息如“我的第一次提交”或者“ 编辑了readme 文件”，等等

```  
6. 链接github上的仓库  
```
git remote add origin https://github.com/你的github用户名/你的github仓库.git  
```  
7. 将本地仓库里的文件推送到 GitHub 仓库（push)  
```
git push origin master
```  
# 参考文献：  
[1]: [d](https://ubuntuqa.com/article/7017.html)


