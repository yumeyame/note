
将当前文件夹进行git初始化
git init
将当前文件夹加入暂存区
git add . 
提交并备注
git commit -m "<name>"
说明一些信息（当前分支为何，与上游分支是否一致，暂存内容与未暂存内容）
git status
注册本地姓名与邮箱地址
git config --global user.name "你的名字"
git config --global user.email "你的邮箱"
# 关联远程仓库
git remote add origin https://github.com/用户名/仓库名.git
# 推送到远程仓库
git push -u origin main
git push
两种将远程仓库克隆到本地的方式
git clone https://github.com/用户名/仓库名.git
git clone git@github.com:用户名/仓库名.git 
两种将文件添加到远程仓库的方式
git remote add origin http://github.com/name/repo.git
git remote add origin git@github.com:name/repo.git
确认远程仓库地址
git remote -v
修改远程地址
（将add改为set-url）
当前文件与最新上传的修改
git diff
查看提交历史与精简版
git log 
git log --oneline
移动到分支并创建
git checkout <name>
git checkout -b <name>
将另一分支与当前分支合并
git merge <name>