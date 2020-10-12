This is a git repo


## – 如何验证Ubuntu上是否安装Git以及在何处安装Git        --参见文献[1]  

```
git --version
```
## - 在Ubuntu上安装和使用Git和GitHub            --参见文献[2][3]
 
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
git add README.md # 添加索引

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
  
8. 下载代码到本地   
```
git clone url
```  
  
  
## - 常见问题              --参考文献[4]-[11]  
  
  
### 参考文献：  
[1]: [Git – 如何验证Ubuntu上是否安装Git以及在何处安装Git](https://ubuntuqa.com/article/7017.html)  
[2]: [初学者指南：在Ubuntu上安装和使用Git和GitHub](https://zhuanlan.zhihu.com/p/44181150)  
[3]: [如何在ubuntu下使用Github？](https://blog.csdn.net/tina_ttl/article/details/51326684)  
[4]: [github常见操作和常见错误！错误提示：fatal: remote origin already exists.](https://blog.csdn.net/dengjianqiang2011/article/details/9260435)  
[5]: [解除GitHub上传文件大小限制](https://www.jianshu.com/p/9ddf90864c89)  
[6]: [github上传“大”文件（25MB以上，100MB以下）](https://blog.csdn.net/AshleyXM/article/details/104766893)  
[7]: [[Git & GitHub] 解决办法：error: failed to push some refs to 'https://github.com/xxxx.git'](https://blog.csdn.net/dietime1943/article/details/79398771)  
[8]: [git pull origin master与git pull --rebase origin master的区别](https://www.cnblogs.com/ellen-mylife/p/12794245.html)  
[9]: [如何重命名Github（Web）中的目录/文件夹？(How to rename a directory/folder in Github(Web)?)](https://www.it1352.com/800293.html)  
[10]: [怎么更改github的某个项目在本地的同步目录](https://www.oschina.net/question/818505_122066)  
[11]: [执行git push出现"Everything up-to-date"](https://www.cnblogs.com/kevingrace/p/6259905.html)  
[12]: [git 下载代码到本地](https://blog.csdn.net/ywl570717586/article/details/79015284)

