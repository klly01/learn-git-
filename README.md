1.安装git  配置用户名和邮箱
	git config --global user.name "Your Name"
	git config --global user.email "Your email"

2.ssh 文件创建   $ ssh-keygen -t rsa -C "youremail@example.com"

3.githup账号下添加 ssh key

4.上传项目 
	创建仓库 -> 本地项目下  git init  ->  
	git remote add origin git@github.com:lxy0828（自己的github名字）/raindrops（自己创建的工程）.git
	-> git add . (or add <filename>)  -> git commit -m"your change description"
	-> git push origin master (or your branch_name)

5.  branch 
	查看当前分支  git branch -r  
	当前分支切换  git checkout <branch_name>
	创建分支      git branch -b <branch_name>
	删除分支      git branch -d <branch_name>

6. 冲突问题
   git fetch：相当于是从远程获取最新版本到本地，不会自动merge
	git pull：相当于是从远程获取最新版本并merge到本地

7.版本切换
  查看版本历程  git log  
  切换版本      git  reset --hard  <hash>
